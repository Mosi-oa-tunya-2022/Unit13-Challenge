# Unit 13 Homework Assignment - The Power of the Cloud and Unsupervised Learning

## Background

It is time to take what you have learned about unsupervised learning and the AWS services and apply it to new situations. For this assignment, you will need to complete **one of two** (not both) challenges. Which challenge you take on is your choice. Just be sure to give it your all -- as the skills you hone will become powerful tools in your FinTech tool belt.

## Option 1: Robo Advisor for Retirement Plans

![Robot](Images/robot.jpg)

_Photo by [Alex Knight](https://www.pexels.com/@alex-knight-1272316?utm_content=attributionCopyText&utm_medium=referral&utm_source=pexels) from [Pexels](https://www.pexels.com/photo/high-angle-photo-of-robot-2599244/?utm_content=attributionCopyText&utm_medium=referral&utm_source=pexels) | [Free License](https://www.pexels.com/photo-license/)_

# Robo Advisor

## Background
This project was created to attract younger investors. I created a robo advisor that could be used by customers or potential new customers to get investment portfolio recommendations for retirement. I combine my Amazon Web Services skills with Python to create a bot that will recommend an investment portfolio for a retirement plan.

### Initial Robo Advisor Configuration: 
I defined an Amazon Lex bot with a single intent that established a conversation about the requirements to suggest an investment portfolio for retirement. 

### Build and test the Robo Advisor: 
I made sure that my bot is working and responding accurately along with the conversation with the user, by building and testing it.


### Enhance the Robo Advisor with an Amazon Lambda Function: 
I created an Amazon Lambda function that validates the user's input and returns the investment portfolio recommendation. This task includes testing the Amazon Lambda function and making the integration with the bot.

##### User Input Validation

- The `age` should be greater than zero and less than 65.
- the `investment_amount` should be equal to or greater than 5000.

##### Investment Portfolio Recommendation

Once the intent is fulfilled, the bot should response with an investment recommendation based on the selected risk level as follows:

- **none:** "100% bonds (AGG), 0% equities (SPY)"
- **very low:** "80% bonds (AGG), 20% equities (SPY)"
- **low:** "60% bonds (AGG), 40% equities (SPY)"
- **medium:** "40% bonds (AGG), 60% equities (SPY)"
- **high:** "20% bonds (AGG), 80% equities (SPY)"
- **very high:** "0% bonds (AGG), 100% equities (SPY)"
