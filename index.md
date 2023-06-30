# Adrijan Parmakovski

**Location**: {{ site.data.about.location }}<br>
**Email**: [{{ site.data.about.email_address }}](mailto:{{ site.data.about.email_address }})<br>
**Phone**: {{ site.data.about.phone_number }}<br>
**Linkedin**: [{{ site.data.about.linkedin_username }}]({{ site.linkedin_url }}{{ site.data.about.linkedin_username }})<br>
**Github**: [{{ site.data.about.github_username }}]({{ site.github_url }}{{ site.data.about.github_username }})

---
## Experience

{% for job_role in site.data.experience %}
<p style="text-align:left;">
    <b>{{ job_role.job_title }}</b><br>
    <b><a href="{{ job_role.company_url }}"><i>{{ job_role.company }}</i></a></b>
    <span style="float:right;">
        <b><i>{{ job_role.duration }}</i></b>
    </span>
</p>
{% for bullet_point in job_role.description %}
- {{ bullet_point }}
{% endfor %}
{% endfor %}

---

## Education

{% for uni in site.data.education %}
<p style="text-align:left;">
    <b>{{ uni.degree }}</b><br>
    <b><a href="{{ uni.university_url }}"><i>{{ uni.university_name }}</i></a></b>
    <span style="float:right;">
        <b><i>{{ uni.duration }}</i></b>
    </span>
</p>
{% for bullet_point in uni.description %}
- {{ bullet_point }}
{% endfor %}
{% endfor %}
