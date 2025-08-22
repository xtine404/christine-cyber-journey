name: Course Tracking
description: Track progress for a cybersecurity course
title: "[COURSE] "
labels: ["course", "planned"]
body:
  - type: input
    id: platform
    attributes:
      label: Platform
      description: Where is this course hosted? (Coursera, TryHackMe, etc.)
  - type: input
    id: link
    attributes:
      label: Course Link
      description: Paste the course link
  - type: textarea
    id: objectives
    attributes:
      label: Learning Objectives
      description: What do you expect to learn?
  - type: input
    id: start-date
    attributes:
      label: Start Date
  - type: input
    id: target-date
    attributes:
      label: Target Completion Date
  - type: textarea
    id: notes
    attributes:
      label: Notes
      description: Extra context, reflections, or links to progress/courses.md
