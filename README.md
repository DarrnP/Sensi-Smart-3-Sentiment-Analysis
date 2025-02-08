# BSC Sensi Smart 3 Sentiment Analysis

# Unguided project

# 
![Image](https://github.com/user-attachments/assets/6b1bcdd4-4818-496a-b568-f8f4ae32d785)
# 


Made a dashboard in Power BI to analyse the sentiment around sensi smart 3 from Bombay 
Shaving Company, by scrapping the reviews of the product from flipkart.

The razor has been marketed as best shaving experience for sensitive skin and very budget friendly but is that truly the case did the customers resonate with that view, I tried to figure it out with this project.

# 
# How I got the data

We can carry out the scraping process by selecting the containers for the various elements in the page and set a for loop to loop through the containers.

Now to extract the required content from the containers we use an inbuilt selenium function find_elements

#
# Scarping the reviews

We can carry out the scraping process by selecting the containers for the various elements in the page and set a for loop to loop through the containers.

Now to extract the required content from the containers we use an inbuilt selenium function find_elements.

Below I have mentioned the py code for the same.

![Image](https://github.com/user-attachments/assets/d24451e2-18ce-4886-bcea-7fa13e9e92ee)


#
# Scarping the date and place of reviews

Used the inbuilt XPATH function to extract the date and place of review together since both were present in the same class ‘row gHqwa8’, then used a try and except clause incase there was no review found at that particular class.

Below I have mentioned the py code for the same.

![Image](https://github.com/user-attachments/assets/84920e6a-cd98-46f2-b2bb-dec2ef6a0520)


#
# Giving each reveiw a sentiment score

To give each review a sentiment score I used Textblob using its inbuilt polarity funciton which gives a polarity. Here polarity is a number lying between [-1,1] where -1 is bad sentiment and 1 is positive sentiment.

Below is the py code for the same.

![Image](https://github.com/user-attachments/assets/bd0e845d-0993-43d1-9448-70c1cd6c8827)
