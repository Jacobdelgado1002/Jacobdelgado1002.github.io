---
layout: page
title: Experience
---


## Research

<script>
function toggleVisibility(id) {
    var x = document.getElementById(id);
    if (x.style.display === "none") {
        x.style.display = "block";
    } else {
        x.style.display = "none";
    }
}
</script>

<table cellpadding="10" width="100%">
{% for research in site.data.research %}
<tr>
    <td width="200" height="100">
        {% if research.image %}
        <img src="{{ research.image }}" alt="{{ research.title }}" width="250">
        {% endif %}
    </td>
    <td>
        <h6>{{ research.title }}</h6>
        <p><strong>Time Period:</strong> {{ research.time_period }}</p>
        <p><strong>Mentor:</strong> {{ research.mentor }}</p>
        <p><strong>Description:</strong> {{ research.description }}</p>
        <p>
            {% if research.details %}
            <a href="javascript:toggleVisibility('details{{ forloop.index }}')">[More Details]</a>
            <div id="details{{ forloop.index }}" style="display:none;">
                <blockquote>{{ research.details }}</blockquote>
            </div>
            {% endif %}
        </p>
    </td>
</tr>
{% endfor %}
</table>

## Extracurricular Activities
Beyond research, I've been actively involved in mentoring and tutoring to support student development:

- **Research Mentor**  
  *Lab:* Edge Computing Group 
  *Duration:* Fall 2024 - Present  
  *Description:* Mentored undergraduate students in the Edge Computing Group by teaching them experiment design and technical writing

- **Tutor**  
  *Course:* Calculus (I, II, and III) and Physics (I and II) 
  *Duration:* Fall 2020 - Spring 2024  
  *Description:* Provided tutoring sessions to help students strengthen their understanding of Calculus and Physics concepts.
