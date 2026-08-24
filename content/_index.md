---
name: "Davis Stapleton"
bio: "I'm a CS student at Syracuse University interested in embedded and backend software. Past work includes HVAC firmware and validation in industrial automation, and automation tooling and database applications in investment management."
description: "Davis Stapleton — portfolio."
links:
  - label: "LinkedIn"
    url: "https://www.linkedin.com/in/davisstapleton"
  - label: "GitHub"
    url: "https://github.com/dtstaple"
experience:
  heading: "Experience"
  items:
    - org: "Johnson Controls"
      role: "Software Engineering Intern, Systems Engineering Team"
      dates: "May–Aug 2026"
      points:
        - "Developed and configured embedded building controllers for system-level testing across networked HVAC devices."
        - "Moved an internal UI regression suite from Selenium to Playwright and cut its runtime by 40%."
      tags: ["Python", "C/C++"]
    - org: "Loomis Sayles"
      role: "Software Engineering Intern, Backend Development"
      dates: "Jun–Aug 2025"
      points:
        - "Built Python and SQL tools to automate reporting and streamline data workflows for the compliance team."
        - "Modernized legacy Perl applications by refactoring code into modular Python."
      tags: ["Python", "SQL"]
projects:
  - title: "CampSite"
    url: "#"
    meta: "Camping trip planner"
    images:
      - src: "/other/campsite.mp4"
        poster: "/other/campsite-poster.jpg"
        zoom: true
    description: "A tool for planning dispersed camping trips. It scores potential sites on things like distance to water, slope, trail access, land cover, and legal status, and writes out a short explanation for each score instead of just plotting dots on a map. It also plans multi-day routes using Dijkstra over a trail graph built from about 334,000 OpenStreetMap segments."
    results: "The OpenStreetMap segments don't share endpoints, so they needed snapping and merging in PostGIS before routing worked."
    tags: ["React", "TypeScript", "Django", "PostGIS", "Mapbox"]
  - title: "Weather Station"
    url: "#"
    meta: "STM32 weather station"
    images:
      - src: "/other/wstation.png"
      - src: "/other/wstationphys.png"
    description: "A weather station built on an STM32 microcontroller. It reads temperature, humidity, and pressure from a BME280 sensor and shows them on a screen, then streams the readings over UART to a Python service that publishes them to an MQTT broker, where a web dashboard subscribes and updates live from anywhere on the network."
    tags: ["C", "STM32 HAL", "I2C/SPI", "Python", "MQTT"]
other:
  heading: "Other Work"
  description: "A mix of smaller projects I've put together."
  items:
    - title: "Serial Debug Console"
      url: "https://github.com/dtstaple/serial_console_v1"
      images:
        - src: "/other/serialconsole.png"
          zoom: true
      blurb: "A desktop serial terminal for debugging microcontrollers. Instead of dumping raw UART text that scrolls by too fast to read, it lays the stream out as a structured table with timestamps, time between messages, and color-coded log levels you can filter."
      tags: ["C++", "Qt6"]
    - title: "PHY 307 computational physics project"
      images:
        - src: "/other/physsim1.png"
          zoom: true
        - src: "/other/physsim2.png"
          zoom: false
      blurb: "A pair of orbit simulators written in C++ for computational physics. One models a single orbit slowly rotating the way Mercury's does; the other runs a multi-planet system, tracking total energy each step to keep the integration accurate over time."
      tags: ["C++", "ffmpeg"]
    - title: "Proof checker"
      images:
        - src: "/other/logicsim.png"
          zoom: true
      blurb: "A tool from my PHI 251 logic class that checks formal proofs written in TFL and FOL. You enter a proof line by line and it verifies each step follows the rules, flagging anything invalid."
      tags: ["HTML"]
---
