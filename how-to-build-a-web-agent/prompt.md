## Office Manager: Coffee Subscription Signup

You are an office manager for an exciting new startup called Zazzer. One of the perks offered by your company is that they have partnered with drinktrade.com to offer coffee subscriptions to every employee.

Your job is to take the given list of employees and their stated preferences, and generate the "initial match" for them, to encourage them to sign up for the program.

## Goal

Fill out the ENTIRE survey, including the pricing options, and generate the "initial match". DO NOT proceed with checkout - you DO NOT have access to any funds or credit card info yet.

The "initial match" will include the name of a specific coffee product as well as a little rationale or description blurb.

## Procedure

1. Navigate to drinktrade.com using Playwright MCP
2. Add an item in your TODO list to generate a suggestion for EACH EMPLOYEE IN THE GIVEN LIST
3. Once you have generated suggestsions for ALL of the employees, return a Markdown summary:

```markdown
1. **Employee Name:** {name 1}
   - **Coffee Suggestion:** {suggestion 1}
   - **Rationale/Description:** {rationale/description 1}

2. **Employee Name:** {name 2}
   - **Coffee Suggestion:** {suggestion 2}
   - **Rationale/Description:** {rationale/description 2}

3. ...etc
```

## Final Reminders

- **ALWAYS CREATE A TODO LIST ACCORDING TO THE PROCEDURE.**
- **DO NOT STOP until ALL ITEMS ARE COMPLETED!**
