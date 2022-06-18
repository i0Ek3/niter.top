+++
author = "i0Ek3"
date = "2022-06-18"
title = "Terrible SPOF"
tags = [
    "SPOF, Google Account, dead loop",
]
categories = [
    "PK",
]

+++

SPOF denotes single point of failure, means a component in a system whose failure causes the entire system to fail. We hear it all the time in RAFT and Byzantine algorithms or distributed systems. Of course, it also happens in our daily life.

Below, I will tell you about the SPOF problems I encountered in my life and how to deal with them.

![ref_spof](https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Single_Point_of_Failure.png/400px-Single_Point_of_Failure.png)


## What I went through?

I've experienced some SPOF-induced events in my daily life, and it's been really scary. Not only did they take my time, they ruined my mood and just "stole" my data.

### 1. Phone issue

When I was young, I only had one phone, I like to install third Android ROMs which I found on XDA. The first part is, this process need to wipe all your data on your phone, I always forget to backup data, so everytime I installed ROM, I need to re-intall all of apps on my phone after that. The point is some files in my phone storage never can be restored after I wipe my data, I just lost them, forever. So, if I backed up the data, I would never have had that situation, but I didn't do that. Second, no one can call me while I'm flashing because I can't answer. If you are unfortunate, the phone will be bricked by your mistake. Fortunately, it is still possible to go around the world without a mobile phone in that time, unlike now, it can be described as impossible without a mobile phone.


### 2. VPN crashed

Somehow, there are some reasons we cannot visit the real Internet directly in China, so the tool is vital. But, in some sensitive times, most tools also cannot work fine, the GFW is so high, normal method cannot through the barrier, you need to build it by yourself. But I didn't do that, cause of my ignorant. I cannot login Google Account anymore in that time, I cannot read my emails on Gmail, most jobs that require real internet cannot be done. But, If I have the other one, maybe it won't be so bad.


### 3. Dead loop

I get two phones, iPhone and Android. I just want to sell my iPhone and reuse Android, so I wiped my iPhone, but I forget quit my Google Account. That's ok, I also can login Google Account on my Android phone without any validations. I just installed PixelExperience Plus ROM on my Andoird phone, but something wrong here, after I installed all apps from iPhone, the Android phone's heat increased highly enough, I am a little scared, so I recovered my Android phone into original ROM, everything is fine, but I forget to quit my Google Account again, yes again. I don't think this is a problem until I cannot login my Google Account anymore.There is a dead loop, for now, I have no device logined Google Account, so I cannot recieve any code from that account. I tried everything I found on Google, but all fails.

The point is, my Google Account bind the Google Voice number as the recover phone number, and I also enable 2FA on my account, all phones wiped, I cannot use any phones to validate the request send by Google, it's a dead loop.

Fortunately, this time I backed up the complete data with a tool before wiping the phone.

That's really a nightmare.


### 4. Keyboard issue

I use hackintosh in my home, I only have a Bluetooth Wired Dual Mode Keyboard on the desk, but the buletooth function always unavailable, and the wired function always unavailable too, I have no idea. When these functions down, I cannot type any words anymore.


## How can I fix it?

After all of the above, I finally realized how terrible a SPOF is. So, basically all the things that may have a SPOF, I have prepared two sets to prevent the loss caused by the single point of failure.

I have two phones, multiple computers, two keyboards, two domains, two Google Accounts and different validation methods, and different tools, almost everything is two, cause of what I experienced.

## What we learned?

Don't be too optimistic, do a good job of data backup, and take measures to deal with SPOF in advance.
