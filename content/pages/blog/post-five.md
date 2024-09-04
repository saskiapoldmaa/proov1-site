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
![](/images/xcet.gif)

Cherenkov detectors, also known by the abbreviation XCET, are gas-filled detectors capable of determining if a charged particle passing through them is above a certain cutoff momentum. If the particle is faster than the phase velocity of light in that gas, the gas will emit light (the principle that nothing can be faster than light applies only to the group velocity of light, not the phase velocity).

The threshold momentum is regulated by the pressure in the detector. The higher the pressure, the higher the refractive index and the slower the light travels in that medium. Hence, to increase the threshold momentum for particles, you need to decrease the pressure.

When you combine two Cherenkov detectors at two different pressures, i.e., you have two different momentum cutoffs for particles to emit light, then you can identify all of the particles in the momentum range specified by the cutoff momenta of each of the detectors. A particle will fall into that momentum range if it emits light in one of the Cherenkov detectors but not in the other.

To map out the momentum of all the particles in the beam, i.e., to measure a spectrum, you need to perform a so-called pressure scan. For this, only one Cherenkov detector is necessary, but you need to vary the pressure in it from the maximum to the minimum. This can be done by initially pumping the detector full of gas and taking measurements while it gradually depressurizes.

During pressure scans, you usually measure the # of particles in a spill that made the medium emit light. You can compare this to the total number of particles in that spill, which is given by the trigger rate.

![](/images/cher1.png)

The x-axis represents the pressure in the Cherenkov detector in bars. On the y-axis is the Cherenkov efficiency.
Cherenkov efficiency is not really an efficiency; it is actually the ratio of particles that emit light to the total number of particles (trigger rate).

As you can see, at low pressure, the threshold momentum is very high, so there are few particles that actually get detected, but as the pressure increases, the momentum becomes less and less discriminating, so more particles are detected.

Pressure scans are more useful after you've translated the x-axis from pressure to threshold momentum.Because particle energies usually follow a normal distribution, the 50% efficiency usually responds to the peak of the spectrum.![](/images/cher2.png)
