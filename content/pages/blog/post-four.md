---
type: PostLayout
title: QDCs
colors: colors-a
date: '2024-02-01'
excerpt: More context that may or may not be helpful
featuredImage:
  type: ImageBlock
  url: /images/featured-Image4.jpg
  altText: Post thumbnail image
bottomSections:
  - elementId: ''
    type: RecentPostsSection
    colors: colors-f
    variant: variant-d
    subtitle: Recent posts
    showDate: true
    showAuthor: false
    showExcerpt: true
    recentCount: 2
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-56
          - pr-4
          - pl-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: center
    showFeaturedImage: true
    showReadMoreLink: true
  - type: ContactSection
    backgroundSize: full
    title: Stay up-to-date with my words ✍️
    colors: colors-f
    form:
      type: FormBlock
      elementId: sign-up-form
      fields:
        - name: firstName
          label: First Name
          hideLabel: true
          placeholder: First Name
          isRequired: true
          width: 1/2
          type: TextFormControl
        - name: lastName
          label: Last Name
          hideLabel: true
          placeholder: Last Name
          isRequired: false
          width: 1/2
          type: TextFormControl
        - name: email
          label: Email
          hideLabel: true
          placeholder: Email
          isRequired: true
          width: full
          type: EmailFormControl
        - name: updatesConsent
          label: Sign me up to recieve my words
          isRequired: false
          width: full
          type: CheckboxFormControl
      submitLabel: "Submit \U0001F680"
      styles:
        submitLabel:
          textAlign: center
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mt-0
          - mb-0
          - ml-4
          - mr-4
        padding:
          - pt-24
          - pb-24
          - pr-4
          - pl-4
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        textAlign: left
      text:
        textAlign: left
---


QDC is a charge to digital converter. This allows you to measure charge that flows through the QDC. 



The graph above depicts the current through the QDC. As you can see, the signal is not at completely 0 when there is no signal, this is due to the noise. For the noise to not contribute, we must pick a very specific integration window, so that only the charge that flew between t\_start and t\_end will be measured.



The green signal here is a trigger signal, it functions as a gate. When it goes LOW, the gate closes and current flows onto one plate of the capacitor. An uncharged capacitor initially acts as a wire, so a fast-enough current signal coming through the gate will simply pass through the capacitor, during which charge accumulates on the capacitor. Then, when the gate closes and the capacitor has just reached its maximum voltage, the ADC comes in to measure that voltage. Here an ADC is just used as a voltmeter. 
What opens and closes the gate? It is a so-called gate generator that gets the signal somewhat earlier than the other components. This is because the signal is delayed before it reaches the gate. The gate generator then recognizes the rise in current and it opens the gate just in time for the signal to arrive at the gate.  On the drawing, there is not only I(t) - our signal coming into the gate. There is also I\_PED - a pedestal current. Its purpose is to get a smaller relative error on the ADC reading and to bring the capacitor into a mode where it is working linearly, i.e where the effective capacitance is the nominal one. 

![](/images/qdc4.png)
