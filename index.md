# Adrijan Parmakovski

**Location**: {{ site.data.about.location }}<br>
**Email**: [{{ site.data.about.email_address }}](mailto:{{ site.data.about.email_address }})<br>
**Phone**: {{ site.data.about.phone_number }}<br>
**Linkedin**: [{{ site.data.about.linkedin_username }}]({{ site.linkedin_url }}{{ site.data.about.linkedin_username }})<br>
**Github**: [{{ site.data.about.github_username }}]({{ site.github_url }}{{ site.data.about.github_username }})
<br><br>

## Experience

{% for job_role in site.data.experience %}
<p style="text-align:left;">
    <font size="2"><b>{{ job_role.job_title }} @ <a href="{{ job_role.company_url }}"><i>{{ job_role.company }}</i></a>, <i>{{ job_role.company_location }}</i></b></font>
    <span style="float:right;">
        <font size="2"><b><i>{{ job_role.duration }}</i></b></font>
    </span>
</p>
<br>
{% for bullet_point in job_role.description %}
* {{ bullet_point }}<br>
{% endfor %}
{% endfor %}