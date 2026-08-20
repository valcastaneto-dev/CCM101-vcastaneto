# Reflection

> Personal reflection on Laboratory Activity 2: Build the
> Cloud Infrastructure Blueprint.

---

If I had to pick the most important cloud infrastructure component from this lab, I'd go with networking. Compute and storage matter a lot too, but none of it means anything if no one can actually reach the server. When I checked the hostname and IP address on my KillerCoda machine, it hit me that this is basically what makes a server "exist" to the outside world. You could have the fastest CPU and endless storage, but without a network connection, it's just sitting there doing nothing for anyone.

This lab also made it click for me why Linux is such a big deal in cloud computing. Running commands like `lscpu`, `free -h`, and `df -h`, I could pull up everything about the server's hardware just from the terminal, no GUI needed. It makes sense that cloud providers lean on Linux so heavily — it's light, free to use, and you can script almost anything, which is huge when you're dealing with hundreds of servers instead of just one.

I also got why documenting infrastructure before deploying anything actually matters, instead of just being busywork. If I had skipped writing things down and just started deploying, I'd probably run into problems later with no idea what the original setup even looked like. Having it all in Markdown means someone else — or future me — could pick this up and understand what's going on without redoing all the investigation.

Skill-wise, I picked up a lot from this one: reading CPU, memory, and disk output from the terminal instead of just running commands blindly, comparing cloud providers side by side, sketching out a basic architecture diagram, and making documentation look clean using Markdown tables and headers.

As for my GitHub, it's looking a lot more legit now. Instead of just one lab sitting there, I've got a second one that's fully documented — README, infrastructure report, component breakdown, provider comparison, the diagram, all of it. It's starting to actually look like something a real cloud engineer would put together, not just a school assignment folder.
