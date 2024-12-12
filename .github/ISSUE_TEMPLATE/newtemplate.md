---
name: Feature
description: "Template for creating feature."
title: "Feature: "
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
        Thanks for taking the time to fill out this bug report!
  - type: dropdown
    id: version
    attributes:
      label: Type of request
      description: Selete the type of your request
      options:
        - New Feature
        - Bug
      default: 0
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: What is the OS which you want to suggest?
      multiple: true
      options:
        - Windows
        - MacOs
        - Linux
  - type: textarea
    id: what-happened
    attributes:
      label: What are the details of your suggestion?
      description: Explain what do you want
      placeholder: Tell us what you see!
      value: "Feature details!"
    validations:
      required: true
---


