---

name: 🐌 Performance Issue
description: Report slow loading, freezing, or other performance problems
title: "[Performance]: "
labels: ["performance", "needs-triage"]
body:

- type: markdown
  attributes:
  value: |
  Is something running slowly or causing problems? Help us make it faster!

- type: textarea
  id: what-is-slow
  attributes:
  label: What's running slowly?
  description: Describe what feels slow or unresponsive
  placeholder: "Example: The page takes 30 seconds to load my data, or the interface freezes when I upload a large file"
  validations:
  required: true

- type: textarea
  id: when-happens
  attributes:
  label: When does this happen?
  description: What are you doing when you notice the slowness?
  placeholder: |
  Example: 1. I go to the data analysis page 2. I upload a CSV file with 10,000 rows 3. The page becomes unresponsive for 2 minutes
  validations:
  required: true

- type: dropdown
  id: frequency
  attributes:
  label: How often does this happen?
  options: - "Every time" - "Most of the time" - "Sometimes" - "Rarely"
  validations:
  required: true

- type: dropdown
  id: device-type
  attributes:
  label: What device are you using?
  options: - "Desktop/Laptop" - "Tablet" - "Mobile phone"
  validations:
  required: true

- type: dropdown
  id: browser
  attributes:
  label: Which browser?
  options: - "Chrome" - "Firefox" - "Safari" - "Edge" - "Other"
  validations:
  required: true

- type: textarea
  id: file-size
  attributes:
  label: File or data size (if relevant)
  description: How big is the file/dataset you're working with?
  placeholder: "Example: 5MB Excel file, or dataset with 50,000 rows"

- type: textarea
  id: screenshot
  attributes:
  label: Screenshot or screen recording
  description: If possible, attach a screenshot or record your screen to show the problem
  placeholder: "Drag and drop your screenshot/video here, or click to upload"

- type: checkboxes
  id: terms
  attributes:
  label: Before submitting
  options: - label: I've checked that this performance issue hasn't already been reported
  required: true
