---
name: Feature
title: "Feature: "
description: "Template for new features."
projects: ["octo-org/1", "octo-org/44"]
assignees:
  - octocat
body:
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: What is your name?
      placeholder: ex. Pongpiphat Kalasuk
    validations:
      required: false
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this feature request!
  - type: dropdown
    id: version
    attributes:
      label: Type of request
      description: Select the type of your request.
      options:
        - New Feature
        - Bug
      default: New Feature
    validations:
      required: true
  - type: dropdown
    id: os
    attributes:
      label: What is the OS for your suggestion?
      multiple: true
      options:
        - Windows
        - MacOS
        - Linux
  - type: textarea
    id: details
    attributes:
      label: What are the details of your suggestion?
      description: Explain what you want.
      placeholder: Tell us what you see!
      value: "Feature details!"
    validations:
      required: true
---
