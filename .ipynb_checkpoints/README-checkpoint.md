# week13_aws_project
In this project, a chat robot that takes in the user's information and recommends a suitable investment portfolio, is built on Amazon Lex .

## Libraries/ library functions
- datetime
- relative delta
- json

## Tools and technologies
- Github
- Gitbash
- Gitlab
- Slack
- Jupyter lab
- Amazon Web Services (AWS)
- AWS Lex
- AWS Lambda
- Xbox game bar screen recorder
- WinZip
- OS: Windows 10 64-bit

## Task
- Create an automated investment recommendation application, if the user satisfies certain criteria and based on the user's risk tolerance

## Initial robot advisor configuration
- A bot 'RoboAdvisor' is created on AWS Lex
- Within the above bot, an intent 'RecommendPortfolio' is created
- Sample utterances are configured to invoke the intent.
- Four slots, 'firstName', 'age', 'investmentAmount' and 'riskLevel' are created to fulfill the intent.
- The 'riskLevel' slot is custom defined, that elicits 4 response cards (risk levels).
- A confirmation prompt is triggered based on the users response.

## Testing the robot advisor
- All the above steps are saved and the bot is built.
- Upon testing, the bot worked as expected

## Enhancing with Lambda function
- To validate the data provided by the user and to recommend an investment strategy based on the risk tolerance, a Lambda function is defined.
- The criteria are: Age must be between 0-65 and the investment amount should be at least 5000 USD.
- The risk levels are: None, Very Low to Low, Medium, High to Very High
- The function is completed, copied to the AWS Lambda and tested with sample test cases.
- The test cases with the wrong information gave the expected errors when run on AWS Lambda.

## Integration/ Testing with AWS Lex
- The Lambda function is integrated with the Lex bot and the confirmation prompt on the Lex is removed.
- The Lex intent is saved and the bot is built to work with the Lambda function.
- The utterances are provided again, and the wrong information in intentionally entered.
- The bot threw the expected prompts and hence, proved that the Lambda function was successfully invoked by the Lex.
- Upon entering all the information correctly, a suitable investment strategy was recommended

## Difficulties faced
- The get_investment_recommendation function was incorrectly defined, at the improper place and the inappropriate value was assigned to be returned.
- The Lambda function was not getting invoked by the Lex bot. When the confirmation prompt was removed, the problem was fixed.

## Project files
- A ZIP folder containing the video recording of the chat interaction
- json file of the AWS intent. (Inside ZIP folder)
- Lambda function Jupyter notebook
- Download the ZIP folder to view the contents.

## Conclusion
- I was surprised to find that my work required very little changes/ corrections and I am looking forward to building more complex projects in the future.

## Contributors
- Satheesh Narasimman

## People who helped
- Khaled Karman, Bootcamp tutor

## References
- https://g.foolcdn.com/editorial/images/501084/risk-meter-with-needle-on-low.jpg

- https://www.realacquisitions.com/wp-content/uploads/2018/10/Blog-Images-300x250.png

- https://download.verafin.com/wp-content/uploads/2018/11/solution-hrc-surveillance-main.png

- https://storage.googleapis.com/crowdnews-media-library/2016/08/photodune-9446388-high-risk-l.jpg

- https://www.youtube.com/watch?v=kpZUN-ae4ts