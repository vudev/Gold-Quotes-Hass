# Gold-Quotes-Hass

Add to config
- platform: rest  
  name: "Gold Quote"
  resource: https://raw.githubusercontent.com/vudev/Gold-Quotes-Hass/main/quotes.json
  value_template: '{{ value_json.quotes | random }}'
#   scan_interval: 3600
  force_update: true
