---
name: "Request a conversation with the Product \U0001F4AC"
about: Request Product to speak with a customer
title: 'Request conversation with Product about TOPIC'
labels: 'conversation-request 💬'
assignees: '@allthedoll'
---

body:
  - type: markdown
    attributes:
      value: |
        Please fill out the form to the best of your ability. 😊
  - type: input
    id: contact
    attributes:
      label: Customer contact:
      description: Which customer contact(s) should we speak with?
    validations:
      required: true
  - type: textarea
    id: topic
    attributes:
      label: Conversation topic(s):
      description: What should we talk about?
    validations:
      required: true
  - type: dropdown
    id: is-demo
    attributes:
      label: Is this a product demo?
      description: |
      options:
        - "Yes"
        - "No"
    validations:
      required: true
- type: textarea
    id: more-info
    attributes:
      label: Anything else to know:
      description: Provide any context, details, etc. that will be helpful.
    validations:
      required: false
