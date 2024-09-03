---
type: PostLayout
title: Varia
colors: colors-a
date: '2021-06-28'
author: content/data/team/doris-soto.json
excerpt: ''
featuredImage:
  type: ImageBlock
  url: /images/featured-Image1.jpg
  altText: Post thumbnail image
media:
  url: /images/post-2.jpg
  altText: altText of the image
  caption: Caption of the image
  elementId: ''
  type: ImageBlock
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
        width: wide
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
CESAR is a software that deals with the beam configuration and also does measurements on a spill level. This means that it can identify the no. of particles in a spill that were counted by xyz detector but it cannot measure anything on a particle level. Hence, in CERN context this is not considered a DAQ (data acquisition system).

TDAQ is a trigger and data acquisition system. This one can do measurements on the particle level.

The no. of particles that you have in the beam is given by two numbers: the event and the trigger rate. Event rate is the one measured by CESAR and this can be taken as the de facto number of particles in a spill. Trigger rate, however, is the number you are actually able to measure with the TDAQ (readout takes some time).

"&" means coincidence, for example S0\&S1\&XCET040 is scintillators 0 and 1 set into coincidence with each other and the Cherenkov 40. 

NIM - nuclear instrumentation module 
