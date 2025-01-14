# NoSQL-Challenge

This challenge involves working with a MongoDB database of establishments evaluated by the UK Food Standards Agency for food hygiene ratings. My task is to clean, update, and analyze this data for the editors of a food magazine.

Acknowledgments

I would like to acknowledge Mee Thao and Susan Thao for their collaboration on this challenge. Their contributions included working together to find out the methods and functions to use on this challenge's file named NoSQL_setup_starter.ipynb.

References
UK Food Standards AgencyLinks to an external site. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I used this website for the to help me find out how to set the Business Type to 1. This is for the NoSQL_setup_starter.ipynb step 13. It specficially helped in providing me these two codes: "update = {'$set': {'BusinessTypeID': '1'}} " and "result = establishments.update_one(query, update)". Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I used this website to help me find out how to delete certain documents from my data. This is for the NoSQL_setup_starter.ipynb step 16. It specficially helped in providing me this code: "establishments.delete_many(query)". Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. I used this website to help me find out what codes to use to change the data type from a string to a decimal for longitude and latitude. It also helped me find out the codes to use to apply the update with aggregation pipeline to only documents with non-numeric latitude/longitude. This is for the NoSQL_setup_starter.ipynb step 19. Accessed on Jan 2025. Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. I used this website to help me find out what codes to use to change the data type from a string to a integer for the rating value. It also helped me find out the codes to use to apply the update for documents where the rating value is still a string. This is for the NoSQL_setup_starter.ipynb step 21. Accessed on Jan 2025. Retrieved fromhttps://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I used this website to help me find out what code to use to check the type of the fields. This is for the NoSQL_setup_starter.ipynb step 22. Specifically, it helped me with this code: "type(document['']['']" Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I used this website to help me find out what code to use to convert the results to a dataframe. This is for the NoSQL_analysis_starter.ipynb step 7. In specific, it helped provide me this code: "pd.DataFrame(establishments.find(query))". Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I used this website to help me find the codes for the NoSQL_analysis_starter.ipynb step 10 and 11 to answer the question: What are the top 5 establishments with a RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?. It helped explain and clarify to me what codes to use and the order to use them in order to get my results successfully. Retrieved from https://chat.openai.com/chat

OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. Accessed on Jan 2025. I sued this website to help me find a code to use for the NoSQL_analysis_starter.ipynb step 13. In specific, it helped me use the aggregate function so that I would be able to print number of documents in the result. The code I used was: "results = list(establishments.aggregate(pipeline))". Retrieved from https://chat.openai.com/chat
