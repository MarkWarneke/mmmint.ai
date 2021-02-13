---
title: Solution Status 
subtitle: >-
  Overview of available solutions, links, documentation and status
solutions:
  - name: Registration Recognition
    description: >-
      This is a description
    dev_docs: https://dev.api.mmmint.ai/fahrzeugschein/v1/docs
    dev_health: https://dev.api.mmmint.ai/fahrzeugschein/v1/health
    prod_docs: https://api.mmmint.ai/fahrzeugschein/v1/docs
    prod_health: https://api.mmmint.ai/fahrzeugschein/v1/health
  - name: Anonymizer
    description: >-
      This is a description
    dev_docs: https://dev.api.mmmint.ai/anonymizer/v1/docs
    dev_health: https://dev.api.mmmint.ai/anonymizer/v1/health
    prod_docs: https://api.mmmint.ai/anonymizer/v1/docs
    prod_health: https://api.mmmint.ai/anonymizer/v1/health
  - name: Numberplate Recognition
    description: >-
      This is a description
    dev_docs: https://dev.api.mmmint.ai/numberplate/v1/docs
    dev_health: https://dev.api.mmmint.ai/numberplate/v1/health
    prod_docs: https://api.mmmint.ai/numberplate/v1/docs
    prod_health: https://api.mmmint.ai/numberplate/v1/health
  - name: Face Recognition
    description: >-
      This is a description
    dev_docs: https://dev.api.mmmint.ai/face/v1/docs
    dev_health: https://dev.api.mmmint.ai/face/v1/health
    prod_docs: https://api.mmmint.ai/face/v1/docs
    prod_health: https://api.mmmint.ai/face/v1/health
  - name: mr fiktiv
    description: >-
      This is a description
    dev_docs: https://dev.api.mrfiktiv.com/v1/docs/
    dev_health: https://dev.api.mrfiktiv.com/v1/health
    prod_docs: https://api.mrfiktiv.com/v1/docs/
    prod_health: https://api.mrfiktiv.com/v1/health
layout: page
---

<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" />

<table>
  <thead>
    <tr>
      <th>Name</th>
      <!-- <th>Description</th> -->
      <th>Development</th>
      <th>Production</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    {% for solution in page.solutions %}
    <tr>
        <td>{{ solution.name }}</td>
        <!-- <td>{{ solution.description }}</td> -->
        <td>
            <a href="{{ solution.dev_docs }}" target="_blank" class="button">
                Documentation: Dev
            </a>
        </td>
        <td>
            <a href="{{ solution.prod_docs }}" target="_blank" class="button">
                Documentation: Prod
            </a>
        </td>
        <td >
            {% if solution.dev_health %}
                <a href="{{solution.dev_health}}" target="_blank">
                    <i class="fa fa-check-circle-o" aria-hidden="true" style="color:#6FB38A"></i>
                </a>
            {% else %}
                <a href="{{solution.dev_health}}" target="_blank">
                    <i class="fa fa-exclamation-circle" aria-hidden="true">
                    </i>
                </a>
            {% endif %}
            |
            {% if solution.prod_health %}
                <a href="{{solution.prod_health}}" target="_blank">
                    <i class="fa fa-check-circle-o" aria-hidden="true" style="color:#6FB38A">
                    </i>
                </a>
            {% else %}
                <a href="{{solution.prod_health}}" target="_blank">
                    <i class="fa fa-exclamation-circle" aria-hidden="true">
                    </i>
                </a>
            {% endif %}
        </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
