This post is all about an assortment of themes that sprout from the same concept,
as could be the deployment architecture of the project, the impact of twitch and
the lauch of the newest **alpha-preview**.

## Dashboard and Servieces
A few weeks ago I lached into the idea of launching a new complied version that could
be tested online, just like I did back during **indev**. The difference here is
that the indev version had little to no security, disregarding any basic access 
exploits or security fails.
This time arround I wanted to focus on security and work towards making this as safe
as posible with my courrent skill and knowladge.

### Arquitecture

![](https://cdn.discordapp.com/attachments/586914620451848234/806988546686713876/Screenshot_2021-02-04_at_21.40.22.png)

Even tho there's some variations regarding the courent arquitecture, the idea of this
serviece is allowing the creation of conections and services to the server so that we
can preform the appropiate deployments while minimizing device access. No, I can't
use stuff like AWS or Azure since the prices have become elevated and I cannot aford
one of those servieces as of now.

This is my first time building a 2FA serviece, and honestly, it has been easier than
I thoguht, after all, every serviece uses the same 6 digit generation, which only 
makes everything even easier. I recomend you implement this in your apps if there's 
any critcal spots, you'll create another layer of security for your login and save
yourself a few headaches later.

### Compilation y desployment.

Even tho I didn't use any Azure machines (or anything similar), Azure Devops allows you
to create Integration Pipelines and deploy them for free, wich despite a few limitations
they are more than sufficiente for the current purpose.
When Mincrosoft bought Github, the allowed for the repositories to be directly connected
with devops, facilitating deployment. Even if they added **Actions**, they don't seems
very usefull compared to Pipelines and DevOps realease systems.

## Twitch

Along with this deployments of Alpha-preview versions, I wanted to let you guys
try this version yourselves, just like with the indev. However, because the Indev
had not been defined as a project, I never really cared about allowing indiscriminate
access to the game. Now though, the future **alpha 1** version might function as
a base for the game, which I actually want to monetize.

### Integration with voidpixel

This integration could be represented with this arquitecture, and it's variations.

![](https://cdn.discordapp.com/attachments/586914620451848234/806988862097195069/Screenshot_2021-02-04_at_21.44.44.png)

The idea is that you can log into the game when you've got a Twitch account with an 
active subscription to my channel over at [Twitch](https://twitch.tv/voidpixelDev).
Game access is done trough [alpha-client.voidpixel.net](http://alpha-client.voidpixel.net/)
It's a simple idea; you click, log into twitch, Boom. You're in.

![](https://cdn.discordapp.com/attachments/586914620451848234/806994449270964254/Screenshot_2021-02-04_at_22.07.36.png)

![](https://cdn.discordapp.com/attachments/586914620451848234/806995219873792040/Screenshot_2021-02-04_at_22.10.12.png)

### Monetization

One of the common coments regarding the game, besides a few Habbo mentions, revolves over the topic
of monetization.
I've given this aspect a lot of thought over lots of times, given that it's an issue I ultimately
have to solve before getting to the point where this thing gets any more serious.
I have been thinking about the next forms of monetization, their pros and cons of each, as well
as my final desition and reasoning.


- **Free To Play (For real)**
  + Good Stuff:
    + Well... it's free.
  + Bad Stuff:
    + Posible account abuse.
    + No source of income.
    + I couldn't work off this.


- **Free To Play (For real) + payed cosmetics**
  + Good Stuff:
    + Free for the user.
    + Options for unique skins
  + Cosas malas:
    + Posible account abuse.
    + Reduced source of income.
    + Dismissive towards some users.
    + I couldn't work off this.


- **Pay to Win**
    + Now, that's comedy.


- **Free To Play (For Real) + optional monthly subscription**
  + Cosas buenas:
    + Free for the user.
    + Options for unique consmetics.
    + I might be able to work off this.
  + Cosas malas:
    + Posible account abuse.
    + Reduced source of income.
    + Dismissive towards some users.


- **monthly subscription**
  + Cosas buenas:
    + Feel_Like_Jeff_Bezos.jpeg
    + Constant source of income.
    + Better average user quality.
    + Could work off this.
  + Cosas malas:
    + Small Userbase
    + Generaly Costly.
    + Will have to do a lot of marketing


- **Pay to play (Once)**
  + Cosas buenas:
    + Semi-Constant source of income.
    + Better average user quality.
    + Could work off this.
    + Fully free experience afterwards, Updates included.
  + Cosas malas:
    + Limits my income
    + Less Userbase
    + Will have to do some marketing

Obviously, you're most attracted to the first option as the reader, but unless I happen
to win the lottery, (which is imposible because I hate chance games) I think not.
I'd like to generate at the very least the suficient amount to recover development
cost, and at most, supposing this happens to function, going ALL IN (mind the irony)
Being realistic towards the idea of my job and living of this in due time, the
last option is the most ethic and coherent to me, therfore the one I'll be using.
**One Payment per account**. For now, we'll wait until the alpha to open this pandora's
box, for now, you can only access the Alpha-Preview trough a Twitch Subscription.

### A rant about Twitch's popularly.

Twitch's popularity since last year is undeniable, I've got this sneaking sensation
that a lot of people "are stealing from me" and even though my head entertains that
idea, I want to make something clear. I know it's not at all like that. 
It's like when you follow a music group that becomes popular and it makes you angry
to see all the new fans and how it became part of popular culture even tho you should
be feeling happy about it.
Otherwise known as this song, which talks precisely about that... In spanish...
So uh... Picture what happened to Dubstep Music, it' was all fine and dandy until 
children started using it for their youtube intros.
[![https://www.youtube.com/watch?v=TGWy14hbIDc](https://cdn.discordapp.com/attachments/586914620451848234/807000489778085958/Screenshot_2021-02-04_at_22.31.32.png)](https://www.youtube.com/watch?v=gBhU2N_Yhhk)

The main differnce between a music group and this twitch fenomenon is that here, just like
in youtube, people can actually become popular and earn enough money to live, it's just
that 99% of them won't get anything, and I fall into this second group. I've been streaming
since 2011, going hard at it since 2013, forgeting a few years of interuption until 2019,
where I got back into it. Since just recently though, it became easier to monetize videos
without having too many followers, allowing us with little audience to earn some money.

And just like it happened with youtube and everything else in popular culture, things peak
then fall. The same thing will happen to streaming. I like finding new people who are
passionate about it like I am, and from here, I encourage you to try it for real.

It just gives me a little sadness to think that this is just a passing trend, and whenever
life gets back to normal, many people who started streaming will stop because they haven't
gained any real income from it. In almost a decade within the platform, it's the first
time I make money, but that doesn't mean I'll stop when it's over, I'll keep going as always,
if you really want to do **Anything**, do it without even thinking about the economic aspects.

Regardless, I want to thank everyone who has been supporting me in he platfrom, weather you've 
been there since 2013, or you're just new. You guys are the reason why Voidpixel keeps going.

Oh, and to add insult to injury, twitch used to have both **Coding** and **GameDev** categories,
Which they've removed. `Make Twitch Great Again` ¡let's get them back!

## Alpha Preview 0.1

As you might have noticed, I've launched the first Pre-Alpha, called `alpha-preview 0.1` on a
tecnicao [sic] level. This version has very little besides the renewed architecture, which I
spoke about [last post](./entity-component-system). Upon further testing, I've found out
that it's much easier to work without the technical problems which have been solved with
this proper distribution of functions and connections between components, which have the info,
entities now only contain relevant information from the components and the systems that
interpret and change all that data. with this amount of scalability and maneuverability, I've
been able to take huge steps towards the evolution of the game.

### Development

The plan for these `alpha-previews` is to mantain a constant flow of "playable" versions and
arrive at the first version with all of the minimal minimums. To reach these minimums, I'll
be making uploads with every development I go on doing.

I thank everyone again for both the good responce to the launch as well as the reading of
this post and all others.
