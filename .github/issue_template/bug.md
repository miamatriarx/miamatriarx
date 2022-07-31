name: Bug Report
description: Report a new bug
title: "Bug: "
labels: ["triage", "bug"]
assignees:
  - miamatriarx
body:
  - type: markdown
    attributes:
      value: Thank you for taking the time to report a bug.  Before creating a new issue have a look at the existing [issues](https://github.com/miamatriarx/miamatriarx/issues) to make sure you don't create a duplicate issue, otherwise rather contribute to the existing issue.
  - type: textarea
    id: bug
    attributes:
      label: Bug
      description: What is the issue?
      placeholder: Provide detail about what you're observing and how it differs from what you expect.
    validations:
      required: true
  - type: textarea
    id: code
    attributes:
      label: Code
      description: Can you provide us with code or a screen shot?
      placeholder: Provide all the code that might potentially be related to the issue, alternatively a screen shot if code isn't possible or relevant.
    validations:
      required: false
  - type: textarea
    id: log
    attributes:
      label: Log
      description: Do you have any useful errors or logs?
      placeholder: Paste the errors or logs you have here.
      render: shell
    validations:
      required: false
  - type: textarea
    id: software
    attributes:
      label: Software
      description: What software are you using?
      placeholder: Provide detail on the software you're using as well as the versions.
    validations:
      required: false
  - type: textarea
    id: information
    attributes:
      label: Additional Information
      description: Do you have any additional information?
      placeholder: Provide any additional information that could be useful to help debug or fix the issue.
    validations:
      required: false
  - type: input
    id: example
    attributes:
      label: Minimal Reproducible Example
      description: Could you provide us with a link to a minimal reproducible example?
      placeholder: https://example.tld
    validations:
      required: false
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: How can we contact you if we need more information?
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
