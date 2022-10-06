---
layout: page
title: Registration
registration_state: closed
email: gapdays2022-summer@gapdays.de
---

{% case page.registration_state %}
{% when 'notyet' %}
<p class="message">Registration will be open soon.</p>

{% when 'closed' %}
<p class="message">Registration is closed.</p>

{% when 'open' %}
<p class="message">Registration is open.</p>

In order to participate in this meeting, please register with us, even if you only want to join for parts of the meeting.

To register please send an email to
[gapdays2022-summer@gapdays.de](mailto:gapdays2022-summer@gapdays.de) with the
following contents.

The registration period for applying for reimbursements ended on July 31, 2022.
We cannot provide reimbursements for new registrations.

The registration will close on September 25, 2022.

```
Registration for {{site.title}}

Name: ...

Email: ...

Affiliation: ... (Please enter the name of your home university, 
institute etc., if any. )

Arrival date: ... (Please enter the day of arrival. We will start 
Monday, October 17, 10 am.)

Departure date: ... (Please enter the day of departure. We will 
finish Friday, October 21, afternoon.)

Mensa Card: Yes/No (Please indicate if you wish to have lunch at 
the university canteen. See Location for more information.)

Child Care: Yes/No (Please indicate if child care is needed. We 
will contact you individually for further details.)

Presentation: ... (If you like to give a presentation during the 
package session please state the title of your presentation.
You are welcome to offer other talks, too.)

Comments: ... (Here you can give any comments, questions, or wishes 
that you have regarding the GAP Days.)
```

If you have any questions
regarding registration, or in general, feel free to
[contact us via email](mailto:gapdays2022-summer@gapdays.de).
{% endcase %}
