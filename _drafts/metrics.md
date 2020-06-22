---
layout: post
title: "To Measure or Not to Measure"
date: 2020-06-23
place: Moscow, Russia
tags: management
description: |
  Individual performance metrics may destroy morale
  and kill teamwork, if being used wrongly, but their
  absence hurts even more.
keywords:
  - performance metrics
  - individual performance
  - metrics
  - performance
  - performance appraisal
image: /images/2020/06/
jb_picture:
  caption: ...
---

The question [was asked](https://softwareengineering.stackexchange.com/questions/26596/metric-by-which-to-hold-developers-accountable)
on StackExchange nine years ago (just around
the time the site was launched): "If not
[lines of code](https://en.wikipedia.org/wiki/Source_lines_of_code), then what is
a good metric by which to measure the effectiveness of remote programmers."
The answers,
[not surprisingly](https://www.youtube.com/watch?v=OOAMNOso46g),
were all along this: programmers are not supposed to be measured!
I bet, those who answered were programmers themselves.
Indeed, [why](https://www.youtube.com/watch?v=sZoJ3gO4PSo)
would a programmer be interested in being measured,
especially with a discreet metric?

<!--more-->

{% jb_picture_body %}

First, let's see why putting a metric on a programmer
may be considered a bad practice (my opinion: these are merely excuses
of overly-paid programmers/managers helping them keeping their jobs, doing
<del>nothing</del> what they want, and wasting employers' money):

  * "Individual performance metrics are against the spirit of Scrum,"
    [says](https://www.scrum.org/forum/scrum-forum/13381/individual-performance-scrum-enviornment)
    [Selçuk Özdoğan](https://www.scrum.org/user/186863).

  * "A hero mindset, if left unchecked, plagues the team spirit,"
    [says](https://medium.com/unboxing-product-management/how-to-reward-individual-performance-in-agile-teams-21dd7bc1a4e2)
    Bhuwan Jain, a Product Manager at [Quovantis](https://www.quovantis.com/).

  * "Performance reviews destroy morale and kill teamwork,"
    [says](https://www.wsj.com/articles/SB122426318874844933)
    [Samuel A. Culbert](https://www.anderson.ucla.edu/faculty-and-research/management-and-organizations/faculty/culbert),
    a professor of management at the
    [UCLA Anderson School of Management](https://www.anderson.ucla.edu/).

  * "Individual rewards fosters competition in an environment
    where co-operation is essential for success,"
    [says](http://www.agilebuddha.com/agile/metrics-to-build-great-agile-teams-measure-influence-not-control/)
    [Avienaash Shiralige](http://www.agilebuddha.com/author/admin/),
    an Agile Coach at [AgileBuddha](http://www.agilebuddha.com/).

  * "Individual metrics discourage team collaboration,"
    [says](https://www.infoq.com/articles/not-destroy-team-metrics/)
    Sean McHugh, a Scrum Master at [Axosoft](https://www.axosoft.com/).

  * "Performance reviews are harmful and completely unnecessary,"
    [says](https://scrumology.com/performance-evaluations-and-scrum/)
    Kane Mar, a co-founder and principal consultant for
    [Scrumology](https://scrumology.com/).

  * "Performance metrics discourage initiative, innovation and risk-taking,"
    [says](https://aeon.co/ideas/against-metrics-how-measuring-performance-by-numbers-backfires)
    [Jerry Z Muller](https://press.princeton.edu/our-authors/muller-jerry-z),
    author of
    [The Tyranny of Metrics](https://press.princeton.edu/books/hardcover/9780691174952/the-tyranny-of-metrics).

  * "Human beings cannot, by their nature, be reduced to a number,"
    [says](https://resources.collab.net/blogs/measuring-individual-performance-can-a-person-be-reduced-to-a-number)
    [Jimi Fosdick](https://www.scrumalliance.org/community/profile/jfosdick),
    a certified Scrum Trainer.

How do you like this? "Keep paying me, but don't expect me to give
you anything back! And don't you dare checking my performance!"---this
is what I hear and I'm not surprised. What's happening is called
the [performance management revolution](https://hbr.org/2016/10/the-performance-management-revolution)
and the gist of it is: modern management is so weak that we desperately
need an official name for this chaos, to avoid confusion. Agile is the name.

Managers are [not in charge]({% pst 2017/aug/2017-08-01-how-to-manage-a-manager %})
anymore, programmers are. And it's only sad.

However, not everybody believes in this anarchy. Some experts think that metrics
are actually helpful. Bradley Kirkman et al.
[claim](https://hbr.org/2016/03/teamwork-works-best-when-top-performers-are-rewarded) that
"recognizing a single team member seems to have a positive and contagious
effect on all the other members in the team,"
and the famous [Vitality Curve](https://en.wikipedia.org/wiki/Vitality_curve)
suggested by [Jack Welch](https://en.wikipedia.org/wiki/Jack_Welch)
in 2001 is still with us.

I believe the all the negativity pointed at metrics is caused by their
incorrect usage. Indeed, if the only performance metric of
software engineers, for example, is the amount of hours they stay in the office,
they will say only bad things about _all_ metrics. Such metrics do hurt, no doubts about this.
But the absence of _good_ metrics hurts even more.
How to chose them---is the right question. Let me suggest a few,
instead of the famous and incorrect LoC.
Ideally, you pick a combination of them from this list, or even use them all together:

  * **Features Delivered**.
    Put a "feature" label to a ticket (or a GitHub issue) and then count
    the amount of tickets closed by a programmer with this label attached.
    Of course, each feature must be closed by a product manager, not
    by the programmer.

  * **Pull Requests Merged**.
    Each pull request has to be peer reviewed to make sure it makes sense
    and adheres to the quality standard of the project. Too small and too
    big pull requests must be rejected.

  * **Bugs Fixed**.
    Bugs work the same way as features, but usually are smaller. The more
    bugs a programmers closes, the better. Of course, closing must be done
    by product managers or other programmers, who report bugs.

  * **Bugs Reported**.
    Once a bug is reported and accepted by the project, the reporter
    must get an extra point. This is how the quality of project grows:
    by [encouraging]({% pst 2018/jul/2018-07-24-bugs-or-pull-requests %})
    everybody to report bugs.

  * **Releases Published**.
    In a disciplined project new versions are released every day, in others
    every week or even months (or never). Every release is a stressful operation
    and it only seems logical to reward programmers for them.

  * **Uptime**.
    There is a set of DevOps metrics demonstrating the quality of
    service in production, including
    [MTBF](https://en.wikipedia.org/wiki/Mean_time_between_failures),
    [MTTF](https://en.wikipedia.org/wiki/Mean_time_between_failures#Variations_of_MTBF),
    [failure rate](https://en.wikipedia.org/wiki/Failure_rate),
    and so on. The longer the uptime, the better the programmers
    and their product.

  * **Cost of Pull Request**.
    The less it takes to merge a pull request submitted by a programmer,
    the better is the programmer, I believe. The faster their PRs
    go through peer reviews and quality control, the better. Junior
    programmers usually submit too big or too complex PRs, causing a lot
    of troubles during peer review. They also cause merge conflicts and
    something even stale branches and never-good-to-merge PRs.

  * **Documentation Pages Published**.
    FAQ pages, JavaDoc blocks, Wiki pages, blog posts, and so on---they help
    the project get closer to users and to future developers by increasing
    maintainability. Of course, every piece of text must be validated
    before publishing.

  * **Mentees Results**.
    Senior programmers may be mentors of more junior ones and may be
    rewarded for the rewards received by their mentees. All metrics listed
    above may work this way, rewarding or punishing mentors when their
    students are doing better or worse.

I can't stress this enough: each metric must have a
[quality control]({% pst 2018/mar/2018-03-06-speed-vs-quality %}) mechanism.
Just measuring bugs reported without checking the quality of them would lead to cheating:
programmers will report whatever they like, just to bump the numbers up.
Each bug must be verified by an architect: duplicates or
[low-quality]({% pst 2018/apr/2018-04-24-right-way-to-report-bugs %})
bug reports are to be rejected. The same is true for every metric:
[trust]({% pst 2019/may/2019-05-28-trust-or-not %}) without control
leads to [cheating]({% pst 2017/nov/2017-11-21-trust-pay-lose %}).

It is also worth mentioning that features,
bugs, pull request, and documentation pages may have different
_complexity_, _urgency_, and _severity_, which also may be taken into account,
increasing or decreasing the numbers in each metric.

Most of these metrics may be collected automatically, without any human
interaction, for example via GitHub API.

In an ideal world of [ideal management]({% pst 2015/jul/2015-07-21-hourly-pay-modern-slavery %}),
the project compensates
the work of its programmers according to the metrics collected. Instead of
salaries, programmers get
[money]({% pst 2014/sep/2014-09-24-why-monetary-awards-dont-work %})
for features, bugs, documentation pages,
and so on. How far is your project from this
[utopia]({% pst 2014/apr/2014-04-17-how-xdsd-is-different %})---is the indicator
of your professionalism as a project manager. [Lousy]({% pst 2017/jun/2017-06-06-gluten-free-management %})
managers don't measure
anything and make everybody "happy" by keeping wages high and control low ...
until the project runs out of money. On the other hand, exceptionally
great managers let metrics
[control]({% pst 2015/oct/2015-10-13-competition-without-rules %})
everybody, making the best happy
and the worst ... [quickly]({% pst 2015/sep/2015-09-16-how-to-fire-someone-right %})
find the way out.

Which one are you?