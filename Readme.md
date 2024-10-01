# Clearview

## Connecting diverse talent to exciting opportunities, removing bias from the process.

This application will revolutionize the way people find jobs and companies find talent. We believe that everyone deserves a fair chance to succeed, regardless of their background. Our platform aims to:

- **Level the playing field**: Eliminate bias from the hiring process by focusing on skills, experience, and potential.
- **Empower diverse talent**: Provide a platform for individuals from all backgrounds to showcase their abilities and connect with opportunities that match their aspirations. Provide AI driven resume writing, fine tuning to he candidates
- **Help companies build inclusive teams**: Enable organizations to access a wider pool of qualified candidates and create a workforce that reflects diversity. Also, help teams by having DEI experts reviewing the interview process and provide feedback


### Key Features:

- **AI-powered resume Matching**: Our intelligent system analyzes resumes for skills, experience, and qualifications, removing unconscious bias from the initial screening process. 
  
- **Personalized resume stories**: We help candidates craft compelling narratives that highlight their unique strengths and career journeys. Provide appropriate resume tips and help them communicate their strengths better. We anonymize the resume and craft stories based on skill, capabilities and experience and share it with the potential employers
  
- **Skill-based matching**: We connect candidates with opportunities that align with their skills and interests, ensuring a good fit for both the individual and the employer.
  
- **Integration with leading HR platforms**: Seamlessly connect with existing HR systems to deliver the interested profiles, streamlining the hiring workflow.


#### Context Diagram

<img src="diagrams/context.png" />



#### Module Diagram


<img src="diagrams/containers-v2.png" />



#### Details

- Even though the UI is depicted in various services, these will be shown to the users (candidates and companies) as a unified portal. Each would be an MFE - Please refer to the ADR's
- Matchmaker will send in the candidate story and the Job details to the LLM and will have the right match + scores


* Some key decisions are in the ADR's







## TODO

   
1. The flow for a DEI supervisors to analyse and give feedback is yet to be developed. It will be a part of version 1.1
2. Define what are the key metrics (a few are)
   1. #of hiring % and rejection %
   2. #Top  3 reasons for Rejection and Hiring
   3. Average Salary per Job level
   
3. Build sequence diagrams for these flows
4. Assumption is a single web based mechanism today for users. We may have an APP later (as we have everything behind API's)
5. Horizontal concerns are common - Observability, Security are common. Build them appropriately as libraries/services
6. Intregrate with Linked and other platforms to pull in required info - to be built in subsequent versions
   



### Team [DUnit]

Ramanan Natarajan , Kaushik Krishnan A and Dwaraknath Bakshi



#### Built for diversitycybercouncil.com

