name: Improvement Request
description: Improvement suggestion
title: "Improvement: "
labels: ["triage", "improvement"]
assignees:
  - miamatriarx
body:
  - type: markdown
    attributes:
      value: Thank you for taking the time to share your idea or suggestions.  Before creating a new issue have a look at the existing [issues](https://github.com/miamatriarx/miamatriarx/issues) to make sure you don't create a duplicate issue, otherwise rather contribute to the existing issue.
  - type: textarea
    id: improvement
    attributes:
      label: Improvement
      description: What would you like to improve?
      placeholder: Explain the improvement as well as the motivation and context, how would it improve or add value to the project.
    validations:
      required: true
  - type: textarea
    id: idea
    attributes:
      label: Idea
      description: Do you have any additional ideas or suggestions?
      placeholder: Provide any additional ideas or suggestions relevant to this improvement.
    validations:
      required: false
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: How can we contact you if we need more information or if we'd like to discuss it?
      placeholder: example@host.tld
    validations:
      required: false
  - type: checkbox
    id: terms
    attributes:
      label: Terms
      description: By submitting this issue you agree to follow our [code of conduct](https://github.com/miamatriarx/miamatriarx/code_of_conduct.md) and that any contribution you make will fall under the [MIT](https://github.com/miamatriarx/miamatriarx/license.md) license, in doing so you agree to our terms and void all claims to intellectual propertly or copyright.
      options:
        - label: I agree to your terms and to follow the community's code of conduct.
    validations:
      required: true
