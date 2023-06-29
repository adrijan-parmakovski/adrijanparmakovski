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
    <font size="2">**{{ job_role.job_title }}** @ **_[{{ job_role.company }}]({{ job_role.company_url }}), {{ job_role.company_location }}_**</font>
    <span style="float:right;">
        <font size="2">**_{{ job_role.duration }}_**</font>
    </span>
</p>
<br>
{% for bullet_point in job_role.description %}
* {{ bullet_point }}<br>
{% endfor %}