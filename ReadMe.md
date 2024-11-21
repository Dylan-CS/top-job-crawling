The reptile practices below are all based on crawling recruitment information from Liepin.com as an example    
      
(1) Use User-Agent to simulate the login state, and realize the continuous replacement of User-Agent types. Note: This method is limited to solving the simple anti-crawler mechanism of some websites, and some websites need to use proxy IP to solve it.  

(2) Crawl the job details page links of all pages of the corresponding job and different regions, and store the crawled links of different jobs in a txt file. The same job can be stored in one file without regions, and each row represents a Details page link. Note: This step requires crawling the job details pages of the same job in different regions, because Liepin.com only lists 10 job directories for a job, and the number of job directories searched for only one region is not enough for our subsequent job requirement analysis.  

(3) According to the details page link of each position crawled in (2), crawl the company’s job requirements for job seekers on the details page and store them in the corresponding txt, and store the same position in a file.    
    
(4) According to the job requirements crawled in (3), the job requirement data is cleaned, and steps such as word segmentation, special symbol removal, and stop word removal are taken to remove information that is not valuable for the current job requirement in the data. Key words are required for the post-cleaned data extraction.    

The results:    
top-job-crawling/tree/main/img_md
![image](https://github.com/Dylan-CS/top-job-crawling/tree/main/img_md/1.png)    
![image](https://github.com/Dylan-CS/top-job-crawling/tree/main/img_md/2.png)
