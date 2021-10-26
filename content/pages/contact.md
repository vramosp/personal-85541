---
title: This is a new page
sections:
  - elementId: contact-form
    colors: colors-g
    backgroundWidth: full
    title: Get in touch
    text: |
      To get in touch fill the form below.
    form:
      type: FormBlock
      elementId: contact-form
      action: /.netlify/functions/submission_created
      destination: ''
      fields:
        - type: TextFormControl
          name: name
          label: Name
          placeholder: Your name
          isRequired: true
          width: full
        - type: EmailFormControl
          name: email
          label: Email
          placeholder: Your email
          isRequired: true
          width: full
        - name: Subject
          label: Subject
          defaultValue: Please select
          options:
            - Error on the site
            - Sponsorship
            - Other
          isRequired: false
          width: full
          type: SelectFormControl
        - name: Message
          label: Message
          placeholder: Your message
          isRequired: false
          width: full
          type: TextareaFormControl
        - type: CheckboxFormControl
          name: updates
          label: >-
            I understand that this form is storing my submitted information so I
            can be contacted.
          width: full
      submitLabel: Send Message
    feature: null
    styles:
      self:
        height: screen
        width: narrow
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-0
          - pb-0
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
    action: /.netlify/functions/submission_created
    type: ContactSection
  - type: HeroSection
    elementId: homepage-hero-1
    colors: colors-f
    backgroundWidth: full
    actions: []
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: left
      subtitle:
        fontWeight: 400
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
layout: PageLayout
---
