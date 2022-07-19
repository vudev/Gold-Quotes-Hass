# Gold-Quotes-Hass
1. Edit quotes (If you want change quotes)
2. Add to sensor
- platform: rest  
  name: "Gold Quote"
  resource: https://raw.githubusercontent.com/vudev/Gold-Quotes-Hass/main/quotes.json
  value_template: '{{ value_json.quotes | random }}'
  scan_interval: 3600
  # force_update: true
