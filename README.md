# Introduction to the command line

This is a template repository for a hands-on session about using the command line with GitHub Codespaces. Create your own copy using the "Use this template" button above.

The goal is to offer a fundamental, but hopefully not too basic introduction to using command-line programs in a cloud-based environment. I'm trying to focus on areas where I've seen people struggle with using command-line programs in the newsroom. 

## Assumptions

This tutorial is intended for use with GitHub Codespaces, which provides a Linux-based development environment in your web browser.

The tutorial portion is oriented around the Bash shell, which is the default in GitHub Codespaces. Most, if not all, of the examples in the tutorial should work on other shells, but if you encounter errors, that may be the reason.

Finally, some of the examples in the tutorial use [csvkit](https://github.com/wireservice/csvkit), which you'll install after you create your Codespace.

## Getting Started with GitHub Codespaces

1. **Create your own repository from this template:**
   - Click the green `Use this template` button at the top of this repository's GitHub page
   - Select `Create a new repository`
   - Give your repository a name (e.g., `my-command-line-tutorial`)
   - Make sure it's set to `Public` (required for free Codespaces usage)
   - Click `Create repository from template`

2. **Open your new repository in GitHub Codespaces:**
   - Navigate to your newly created repository
   - Click the green `Code` button on your repository's GitHub page
   - Select the `Codespaces` tab
   - Click `Create codespace on main`
   - Wait for the environment to load (this may take a minute or two)
   - csvkit will be automatically installed during setup

3. **Open the terminal:**
   - Once Codespaces loads, you'll see VS Code in your browser
   - Open a terminal by clicking `Terminal` > `New Terminal` in the menu bar
   - Or use the keyboard shortcut `Ctrl+Shift+\`` (backtick)
   - Copy and paste this command into the Terminal:

   ```bash
   go install github.com/maaslalani/slides@latest
   ```

   It will take a minute to run. You won't have to do it again.

4. **Navigate to the tutorial:**
   ```bash
   cd tutorial
   ```

5. **Start the tutorial:**
   - Open `tutorial/README.md` in the VS Code editor to follow along
   - You can edit this file directly to record your answers as you work through the exercises
   - You can also view `tutorial/solutions.md` for reference

6. **Tutorial reflection:**
   At the end of this README, answer the following questions:
   - How could command line skills improve your efficiency as a journalist?
      
      i think it really goes back to what you said earlier: a lot of journalism is about counting. i’ve always used r for data stuff, and i love r, but the command line in some ways does seem more intuitive lol. of course, i'm sure there are certain advantages/disadvantages to both, but they both serve generally the same function in journalism, right? to analyze data — everything from numbers to text. and if this could improve my efficiency as a data journalist, specifically, i’m all ears. i feel like i sometimes spend so long trying to get an r chunk to work that im ready to leak brain cells out of my ears. like, oh my god, using arrows to fetch an old prompt? *.csv?? cd .. ??? TAB COMPLETION???? a. m. a. z. i. n. g. those things alone would likely cut in half the time it takes me to do some of the tasks i currently use r for. 

   - What types of stories or investigations would benefit most from these tools?
      
      i mean, my love of r is rooted in my love for enormous datasets — particularly when it comes to money stories or trend tracking. but even from the little ive used it, the command line seems considerably more efficient than r. it was so much easier to execute searches across datasets, something that, in r, requires a bunch of str_detect() and r_bind(). for me personally, i think this would allow me to do things faster. i’m working with a lot of money data right now for cns — like, really big figures — and this does seem more manageable and maybe slightly less infuriating than r. speaking about journalism in general, i think any good data story (i.e. any story that cannot be contained in a google sheet) can benefit from tools like this that provide programmatic analysis and allow you (and editors) to trace and thus fact-check your steps. i also think this seems super helpful for short turnaround stories — particularly for getting quick summary statistics on really big datasets.

   - What felt most challenging about learning these technical skills?

   i mean, the biggest thing is learning a new language. i can somewhat competently stumble around in r, but that took a while, and i’m used to the syntax. i will note that when i tried to take your class in the spring (lol) and we looked at the command line, i got really nervous. and then i dropped the class, so it was fine (well, that part was, anyway). and looking at it again on monday gave me the same ick factor. but honestly? it was super intuitive — to the point where i was guessing how to do something based on how i had done something else. with most of it, i kind of just played around with the syntax until it did what i wanted, and i could usually troubleshoot my way through it by myself (or with a very quick google search). which made me feel super smart, btw — great feeling. so maybe im not that nervous about learning it anymore?

   - How does this connect to your understanding of data journalism?
   
   i dont know. do “real” (sorry) data journalists use the command line for stuff? i feel like this seems super helpful to me, but im kind of a moron, so what do i know? it just doesn’t feel like this gets talked about very much, that’s all. but from my perspective, this connects to data journalism in a lot of ways: it’s an intuitive tool that allows you to load large sets of data, somewhat quickly figure out what you’re looking at and then analyze it — both on its own and in conjunction with other datasets — to find compelling data-driven story angles. i’m going to be honest, i wasnt exactly sure how it connects to ai. BUT. then i remembered i’m pretty sure that’s how you connect to an ai api, which is how you train models … ?

## What's in here?

- `tutorial`: Instructions and data for the hands-on activity we'll walk through during the conference session. You should also be able to follow along on your own computer.
- `tutorial/slides.md`: Slides used during the conference session. These can be displayed using the [slides](https://github.com/maaslalani/slides) tool.
- `tipsheet.md`: General tips and links to other references for using the command line.

## Data sources

The command line is by no means a set of tools and concepts specific to journalism. I've tried to use real data in this tutorial to ground the concepts in the kinds of ways I use the command line as a data reporter.

### ICE Detention Statistics 

Agency: U.S. Immigration and Customs Enforcement

Link: [Detention Management | ICE](https://www.ice.gov/detain/detention-management)

### National Population Totals and Components of Change: 2010-2019

Agency: U.S. Census Bureau

Link: [National Population Totals: 2010-2019](https://www.census.gov/data/tables/time-series/demo/popest/2010s-national-total.html)

### National Population Totals and Components of Change: 2020-2024

Agency: U.S. Census Bureau

Link: [National Population Totals: 2020-2024](https://www.census.gov/data/tables/time-series/demo/popest/2020s-national-total.html#v2023)

### UMPD Incident Logs

Agency: UMPD

Link: [UMPD Incident Logs](https://umpd.umd.edu/statistics-reports/daily-crime-and-incident-logs)
