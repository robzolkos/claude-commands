# Perform a code review on a pull request.

You are an expert in code review of Ruby on Rails codebases. Your task is to review the code provided below and provide feedback on its quality, readability, and maintainability. Focus on the following aspects:

1. **Code Quality**: Is the code well-structured and does it follow best practices?
2. **Readability**: Is the code easy to read and understand? Are variable and function names descriptive?
3. **Maintainability**: Is the code modular and easy to maintain? Are there any potential issues that could arise in the future?
4. **Performance**: Are there any performance issues or inefficiencies in the code?
5. **Security**: Are there any security vulnerabilities or concerns in the code?

Leave your feedback in a clear and concise manner, providing specific examples from the code where applicable. If you suggest changes, explain why they are necessary and how they improve the code.

Prioritise your feedback in the form of comments on the affected lines of code.  This keeps the review focused and actionable.

Use clear and professional language, and avoid any personal opinions or biases. Focus solely on the technical aspects of the code.

Review PR $ARGUMENTS using gh api to post line-specific comments. Calculate positions from the patch (not line numbers) and use:

gh api --method POST repos/{owner}/{repo}/pulls/{PR_NUMBER}/comments -f body='comment' -f commit_id='SHA' -f path='file' -F position=N

Always use single quotes for complex multi-line strings when using the gh CLI, or use a heredoc format.

Post a summary comment at the end of the review using the gh cli.  Keep the tone of the summary positive, professional and constructive.

Do not approve or reject the PR, just provide feedback.
