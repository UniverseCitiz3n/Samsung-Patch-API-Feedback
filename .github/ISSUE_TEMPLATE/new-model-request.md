---
name: New model request
about: Request for new model to be included in database
title: "[NEW MODEL]"
labels: new model
assignees: ''

---

name: "📱 New Model Request"
description: "Request to add a new Samsung device model to the API."
title: "[New Model] <Device Model Name>"
labels: ["new model"]
body:
  - type: markdown
    attributes:
      value: "## 📌 New Model Request\nPlease provide the necessary details below to request a new Samsung model."

  - type: input
    id: model_number
    attributes:
      label: "📱 Model Number"
      description: "Enter the full model number (e.g., SM-G991B)."
      placeholder: "SM-XXXX"

  - type: input
    id: csc_code
    attributes:
      label: "🌍 CSC Code"
      description: "Enter the country-specific code (e.g., EUX, XEO, DBT)."
      placeholder: "EUX"

  - type: checkboxes
    id: confirmation
    attributes:
      label: "✅ Confirmation"
      description: "Please confirm the following:"
      options:
        - label: "I have checked the API and confirmed this model is not already listed."
          required: true
        - label: "I understand that the addition of this model may take time."
          required: true
