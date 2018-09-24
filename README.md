# SANLUCSDE001

This challenge required me to scrape the 8 most recent posts from Expedia's Facebook page. I first had to decide what language and tool to use. First, I choose Python because of my familiarity with the language. I next did research on with scraping tool to use and I finally landed on using beautifulSoup. In order to scrape the website I had to first familiarize myself with the DOM; I did this by stepping through the HTML using the dev console. I loaded the HTML using beautiful soup and began to "grad" the required information using the class and HTML tags. Because I knew the limit of posts to scrape I knew that I could just "grab" the post using the correct class and using the built in method of .find_next. I traversed it similar to a linked list where I began at the Head node and with each loop I reassigned the current node as the .next node, I could do this how ever many times I wanted using a while loop or recursively. I choose to do it recursively because I only had to grab 8 elements so the stack trace wasn't a concern. I created the data in the shape that I wanted in each loop by first instantiating a global posts_list array and in each loop I instantiated an empty current_post object, for each object I placed a key value pair corresponding to the necessary information at the end of each loop I appended the current object to the global posts array. Once the function finished running I was ready to write the data to a separate file. I used a built in Python method for writing into files however my script is dumping json the method I found is cross compatible.