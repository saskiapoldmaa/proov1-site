---
type: PostLayout
title: Cherenkov detector
colors: colors-b
date: '2024-05-02'
excerpt: more context
featuredImage:
  type: ImageBlock
  url: /images/featured-Image5.jpg
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
Cherenkov detectors, also know by the abbreviation XCET are able of determining if a charged particle that passes through it is above some cutoff momentum. If the particle is faster than the phase velocity of light in that medium (it's fine only because it's phase not group velocity), then the medium will emit light.  When you combine two Cherenkovs which are at two different thresholds, then you can identify all of the particles in one specific momentum range, because such particles will emit light in one of the detectors but not the other. 

The threshold momentum is regulated by the pressure in the detector. The higher the pressure, the higher is the refreactive index and the slower is light in that medium. Hence, to increase the threshold momentum for particles, you need to decrease the pressure. 

To map out the momentum of the particles, i.e to measure their spectra, one needs to do a so-called pressure scan. For this, you only need one Cherenkov but you need to vary the pressure in it from maximum to minimum. This can be done by just pumping the detector full of air and waiting while taking measurements until it runs out slowly.

During pressure scans, you usually measure the no. of particles in a spill that made the medium emit light. You can compare it to the total no. of particles in that spill, which is given by the trigger rate. ![](/images/cher1.png)

The x-axis is pressure in the Cherenkov in bars. On the y-axis is the Cherenkov efficiency. Cherenkov efficiency is not really an efficiency, it is actually the ratio of particles that emit light to the total number of particles (trigger rate). As you can see, at a low pressure the threshold momentum is very high so there are few particles that actually get detected.Pressure scans are more useful after you've translated the x-axis from pressure to threshold momentum.Because particle energies usually follow a normal distribution, the 50% efficiency usually responds to the peak of the spectrum.![](/images/cher2.png)
