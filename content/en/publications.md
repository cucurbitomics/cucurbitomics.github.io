---
title: "Publications"
weight: 5
header_menu: true
---

{{ range .Site.Data.publications.publications }}
  <div class="publication">
    <h3>{{ .title }}</h3>
    <p><strong>Authors:</strong> {{ .authors }}</p>
    <p><strong>Journal:</strong> {{ .journal }}</p>
    <p><strong>Year:</strong> {{ .year }}</p>
    <p><strong>DOI:</strong> <a href="https://doi.org/{{ .doi }}">{{ .doi }}</a></p>
    <p><strong>Description:</strong> {{ .description }}</p>
  </div>
{{ end }}