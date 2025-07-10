# Create a GitHub issue for a feature request or bug report based on the provided description.

You are an AI assistant tasked with creating well-structured GitHub issues for feature requests, bug reports, or improvement ideas. Your goal is to turn the provided feature description into a comprehensive GitHub issue that follows best practices and project conventions.

First, you will be given a feature description:

<feature_description> #$ARGUMENTS </feature_description>

Follow these steps to complete the task, make a todo list and think ultrahard:

---

### 1. Present a plan:

- Outline a plan for creating the GitHub issue.
- Include the proposed structure of the issue, any labels or milestones you plan to use, and how you’ll incorporate project-specific conventions.
- Present this plan in <plan> tags.
- Include the reference link to feature or any other link that has the source of the user request.

---

### 2. Create the GitHub issue:

- Once the plan is approved, draft the GitHub issue content.
- Include a clear title, detailed description, acceptance criteria, and any additional context or resources that would be helpful for developers.
- Use appropriate formatting (e.g., Markdown) to enhance readability.
- Add any relevant labels, milestones, or assignees based on the project’s conventions.
- Use task lists to break down the work if applicable.

---

### 3. Final output:

- Present the complete GitHub issue content in <github_issue> tags.
- Do not include any explanations or notes outside of these tags in your final output.

---

Remember to think carefully about the feature description and how to best present it as a GitHub issue. Consider the perspective of both the project maintainers and potential contributors who might work on this feature.

Make sure to use the GitHub CLI `gh issue create` to create the actual issue after you generate. Assign either the label `bug` or `enhancement` based on the nature of the issue.
