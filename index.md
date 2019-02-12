---
title: Test title
layout: post
---

## One Man and His Machine: Random Musings and Memory Dump

### January 22, 2019

> The economics of software security: This is why we can't have nice (secure) things.

This strategy tends to fail economically. The tech startups that succeed are usually ones that let their customers do things they would not otherwise be able to do. Usually doing something that nobody has done before is hard enough without considering the corner cases; if it follows a typical 90/10 rule, then doing 100% of the job will take 10x as long as the competitor who's only doing the easiest 90%, and your market will have been snapped up by them long before you can release a product. Customers would rather use a product that works 90% of time than do without a product entirely, at least if it delivers functionality they really want but can't get elsewhere (and if it doesn't, your company is dead anyway).

Once you've got a commanding lead in the marketplace you can go back and hire a bunch of engineers to finish the remaining 10% and make it actually work reliably. That's why solutions like testing & exceptions (in GCed languages) succeed in the market: they can be bolted on retroactively and incrementally make the product more reliably. It's also why solutions like proof-carrying code and ultra-strong (Haskellish) typing fail outside of markets like medical devices & avionics where the product really needs to work 100% at launch. They force you to think through all cases before the program works at all, when customers would be very happy giving you (or a competitor) money for something 80-90% done.

Someday the software market will be completely mature, and we'll know everything that software is good for and exactly what the product should look like and people wouldn't dream of founding new software startups. At that point, there'll be an incentive to go back and rewrite everything with 100% solid and secure methodologies, so that our software has the same reliability that airline travel has now. That point is probably several decades in the future, though, and once it happens programming will not be the potentially extremely lucrative profession it is now. 

> Here is a similar line of argument with a different example. 

MongoDB didn't become a public company through innovations in fundamental distributed database technology or even through good engineering. They became a public company because once Javascript became adequate for building client software, there was a strong incentive to build MVPs using the same data structures from client to server to DB, and once you build an MVP that gets adoption there's a strong incentive not to switch databases.
That's the sort of shift in the environment that the grandparent is talking about. Fundamental CS tech was arguably better in the 1970s and 1980s, because it moved more slowly and you had time to get the details right. That doesn't matter if you're building say a mobile Ethereum wallet in 2018, because you're building for the user expectations of today, they don't care about data integrity or security as long as it doesn't fail during the period where they're deciding which tech to use, and software that solves the problem (poorly) now is better than software that doesn't exist. 

Nobody wants to pay for security, but eventually we will all pay the price. Here's [another discussion](https://news.ycombinator.com/item?id=19143928).

Feb 8: For consumers there exist several fine VPN solutions such as AirVPN, PIA, [PrivateTunnel](https://www.privatetunnel.com/), Mullvad, ProtonVPN and Windscribe which offer reasonable service at reasonable price, if you don't want to go to the trouble of rolling your own. (because maintenance and upkeep!) I also recommend checking out [Streisand](https://github.com/StreisandEffect/streisand) which served as the foundation of Canadian Shield VPN, which is presently defunct in this highly competitive and increasingly commoditized arena where I would expend my (at this point) limited personal resources trying to play catch up with no meaningful competitive advantage for most consumers. Without raising funding it is difficult to support all major platforms and basically I would compete at a significant disadvantage without sacrificing more than I can presently provide.

The business model is proven and is profitable, scales well, and requires very little starting capital (to the point where you can bootstrap) which is why everyone is doing it. SurfEasy, TunnelBear and Windscribe are three Canadian firms who have grown with the market and the former two were recently acquired by [Symantec](https://investor.symantec.com/About/Investors/press-releases/press-release-details/2017/Symantec-Announces-Acquisition-of-SurfEasy-Inc/default.aspx) and [McAfee](https://www.tunnelbear.com/blog/tunnelbear_joins_mcafee/) respectively. And that's just here in Canada. (basically Toronto) 

So that's my story and I can elaborate on the gory details upon request. If you want a good narrative, I can recommend reading: [Reflecting on My Failure to Build a Billion-Dollar Company ](https://news.ycombinator.com/item?id=19105733) which is about as ridiculous as it sounds. 

Remember one day, you will be dead. With each year that passes after your death, fewer and fewer people will remember who you were, what you did or what your face looked like. Eventually, you'll be completely forgotten. Who cares if that side project you put out sucked or not. Might as well put it out there and see what people think. There's a good chance too that the project won't even be remembered even by the time you die. The best way to get experience is to do things, so given that no one is going to remember, might as well try to do it. Your successes won't be remembered along with your failures.

### January 11, 2019

I wanted to share this interesting article: [Most of What We Read on the Internet is Written by Insane People (reddit.com)
](https://news.ycombinator.com/item?id=18881827)

The key takeaway for me was the following:
> If you consume any content on the Internet, you're mostly consuming content created by people who for some reason spend most of their time and energy creating content on the Internet. And those people clearly differ from the general population in important ways.

The post itself is worth a read and there are many interesting comments in the discussion.  
> When Rome's military went from citizen soldiers to full time specialist professionals, the misalignment of incentives between the specialists and the citizens was the subtle, long term root of many problems. 
I think this is the case with programmes as a profession, as hacker culture is diluted by more mainstream commercial interests. The easy money in ad-tech has attracted brogrammers as our standards and expectations for privacy and security seem to decrease with each passing year.

Many of my friends are exceedingly optimistic about the potential and possibilities in technology but sometimes I wonder if we are really moving forward but taking two steps back. For example I prefer to remain annonymous and keep private as much as possible. I believe most of us would see the right to ownership of property as inalienable and the right to privacy and security is (arguably) no less important, but this is increasingly being erroded in an age of [surveillance capitalism](https://en.wikipedia.org/wiki/Surveillance_capitalism)

This unfortunately goes against the zeitgeist in an time where it is popular to [write essays](https://www.linkedin.com/pulse/leaving-microsoft-paul-richardson/) to announce a departure from a job, share what you ate for lunch on Instagram/Facebook/Github and even personal blogs to some extent have become vechicles for self-promotion and marketing/storytelling. 

> This is why I constantly work to become a better storyteller, both for personal and professional reasons. You must promulgate the narrative surrounding yourself and your work or someone else will.


Time spent talking about your work is time you could be spend getting things done. Unfortunately humans absolutely require a narrative surrounding anything with which they consider themselves associated with. It’s vastly superior to that being one provided by you (by human resources, hiring managers) versus one invented for use by those who know you. So here I am writing a blog entry, I hope you enjoy the story.

### January 9, 2019
I've been playing around with Jekyll for two days and it is unfortunate that I have to install some Ruby packages like Bundler if I wish to [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#step-2-install-jekyll-using-bundler) This could all be done within a VM but I also find the workflow and Jekyll itself to be rather cumbersome. So for now I am forced to test changes by pushing directly to production, sometimes without of even previewing my changes. In 2019 there must be some better alternative!

### January 7, 2019
Hello world, today a blog is (re)born! Incidentally GitHub has announced unlimited private repositories for free users so that might have something to do with it! See [Reddit](https://www.reddit.com/r/programming/comments/adjw6g/github_now_gives_free_users_unlimited_private/) and [HN](https://news.ycombinator.com/item?id=18847043). I don't plan to blog so much as dump random snippets and notes on things I've read. Previous incarnations of my website appeared in the form of a [Hatta Wiki](http://test.hatta-wiki.org/) but I suppose the collaborative nature of Github suits this purpose well. Markdown is still supported so the [basic writing and formatting syntax](https://help.github.com/articles/basic-writing-and-formatting-syntax/#links) will be familiar.

["If a tree falls in a forest and no one is around to hear it, does it make a sound?"](https://en.wikipedia.org/wiki/If_a_tree_falls_in_a_forest) I suppose people are curious regarding my relative silence and a "narrative" is required but that will be for another post. For now I will leave you with a question and answer. [Ask HN: How to found a company as a single founder?](https://news.ycombinator.com/item?id=18855704) and [Seven tough lessons from ten years in bootstrapped business](https://news.ycombinator.com/item?id=18582553). They are long reads but dig in if you really want the answer to your question.

These days my main interest is in cybersecurity and that will be my focus of my writings in this blog. They say: "Premature optimization is the root of all evil" and I share similar sentiments regarding complexity about blogging platforms. Hardware, software, platforms, and ecosystems are often unnecessarily complex and many of our security, privacy, and abuse problems stem from that. So a simple, static website hosted on [Github Pages](https://vinc456.github.io/) should suit my needs and my hope is there will be little to no maintenance so I can focus on writing. My hope is that this be the ;ast blogging platform I will ever need to setup/learn/maintain but the only thing one can bet on in technology is relentless change....  

###### Random Readings

[The State Of Software Security In 2019](https://www.reddit.com/r/security/comments/adkvu1/the_state_of_software_security_in_2019_and_what/)

Interview with Mark Russinovich-the future of Sysinternals 3/5. [Sad state of security, as an intractable problem](https://youtu.be/3-kjale0tDk)

> Dependency slurping systems like NPM, CPAN, go get, and so on continue to freak me out. They might potentially be more dangerous than manual dependency management, despite the huge risks of that practice, precisely because they make it ‘easy’ to grow your project’s dependency graph — and hence the number of individuals and organizations that you implicitly trust. (And their trustworthiness can suddenly change for the worse.) When there are significant gaps in a language’s standard library, third-party developers will eagerly fill those gaps with new dependencies for you to (not always knowingly) inherit. There is an effort underway to fill gaps in JavaScript’s standard library, which I strongly support for this reason.
[Dependency resolution is a good application of topological sorting.](https://www.quora.com/What-is-topological-sorting
)
