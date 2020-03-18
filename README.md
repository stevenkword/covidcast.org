# covidcast.org
Trying to help with what I've got.

If you represent a government, health organization, publisher or non-profit and are on a mission to propagate helpful and verified factual information regarding COVID-19 across your existing (or exploring new) channels, I would like to offer my services, free of charge. What do YOU need?

As I write this, I realize this offer won’t scale, so I'll be looking for a little help from my opensource friends (that IS LIKELY you).

-- Inspired by Muneer Nawab’s post: https://www.linkedin.com/pulse/6-devs-2-designers-3-pms-marketers-dreamers-how-can-we-muneer-nawab/


## The why  (PR’s encouraged!):

It’s not JUST about “France”, it’s ALSO about the “Francophone nations”.  While working with the AWS text-to-speak SaaS application, Polly, back in 2018, I specifically remember an EMS use case mentioned in one of the case-studies.  There was a Tsunami in Indonesia, and the information distribution system we all expected was handcuffed.  Through a combination of electric generators, translation capabilities, and execution, they were able to get real-time updates from those in the know to those who were not --- using an old technology most of us had forgotten about,  FM Radio.  The culture was split linguistically, and the intersection of emerging technologies and good ol’ human kindness saved lives.  Let’s not let that lesson go to waste while we’re all sitting around acclimating to our new work-from-home offices from the comfort of the first-world. To be clear, that is not a statement of judgement, however it is a commitment to not turning a blind-eye.

##The How (PR’s Welcome!)

Single page headless application.  Electron comes to mind!
WordPress backend -- Content management is what it does best and it natively publishes REST endpoints that are easy to manage.
The Atlantic has published an API for verified data on a per state basis:
Custom WP-CLI command to “update_post” based on a JSON object, initiated by a bash call to WP-CLI on a cron. This would make a server-side async call to the API.  Caching is inherited by the WP APIs.
Leverage one of my old friends, AWS for WP, which bundles Amazon Polly and Amazon Translate.  There are hooks on “update_post” to facilitate this behavior.

