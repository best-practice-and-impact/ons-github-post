# Gitting the most out of version control

## Git at the ONS

[Git](https://git-scm.com/) is a version-control system for tracking changes in a collection of files, called a repository. It works best for text-based files like code but can be used to version-control any file type. It provides additional features that support multiple people working on the same files within a project, whilst creating an audit trail for all changes to those files. This means that you don’t need to manually keep copies of file versions, for example by saving them with a new name: “some_code_v3_new_final.py”.

<p align="center">
  <img src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png" alt="Git Logo" width="20%" />
</p>

This form of version control is particularly useful when carrying out analysis using coding tools, such as Python or R. You're able to save collections of related changes (called commits), resolve conflicts between changes from multiple users and effortlessly roll back to earlier versions of the project or individual files. This is essential for reproducing outputs from previous versions of your analyses. You can find an [introduction to Git course](https://learninghub.ons.gov.uk/course/view.php?id=532) and [screencast](https://learninghub.ons.gov.uk/enrol/index.php?id=782) on the Learning Hub, or more detailed usage in the online [Pro Git book](https://git-scm.com/book/ru/v2).
 
Last month a new version of Git (v2.27) was rolled out to users across the ONS. 
 
Git forms the basis of several version control platforms. You may have experience using Git to version control your projects on the ONS GitLab platform, or equivalent in the Data Access Platform (DAP). An update to the system level configuration of Git now enables ONS machines to connect to [GitHub](https://github.com/) - the world's leading software development platform. GitHub provides very similar features to GitLab but allows us to easily share work between government departments and even publicly. It provides tight control over access for viewing and contributing to each project, so that code can still be kept private when necessary.
 
This form of version control is a core element of Reproducible Analytical Pipelines (RAP), which automate analytical processes. The Centre for Crime and Justice (ONS) have recently moved versioning of the code for their recently developed RAP to GitHub. This code has been used to produce the latest “Nature of Crime” statistical tables. You can read more about their [RAP development and use of Git](https://gss.civilservice.gov.uk/blog/the-nature-of-rap/).

## Open source

[Open source](https://opensource.com/resources/what-open-source) describes software for which the source code is freely available for use, which can be modified and redistributed.

>*"Make all new source code open and reusable, and publish it under appropriate licences. Or if this isn’t possible, provide a convincing explanation of why this can’t be done for specific subsets of the source code."*
>
> --- [Government Service Manual](https://www.gov.uk/service-manual/service-standard/point-12-make-new-source-code-open)

Whenever possible, we should open source the code behind our analyses and statistics. This practice promotes collaboration and innovation, which are core elements of our current strategy. Doing so is beneficial for ONS-based programmers, developers in other departments and the public. These benefits include:
 
Personal development:
* Attribution - coding in the open creates a public record of your contributions to software, as evidence of your programming skill
* Collaboration - you can gain experience working with other programmers
* Review - peers and experts in the field can provide advice on developing your code further
* Satisfaction - it's nice to be able to give back to the community that provides software that we all use on a day to day basis

Public good:
* Transparency - users can understand and reproduce our analysis, which is a core element of the [Statistics Code of Practice](https://code.statisticsauthority.gov.uk/)
* Shared value - others can benefit from using your code and won't have to reinvent the wheel
* Shared opportunity - others can gain insight and experience from reading and possibly even contributing to your code

As with all documents that the civil service publish, there are [security considerations to be made when releasing code publicly](https://www.gov.uk/government/publications/open-source-guidance/security-considerations-when-coding-in-the-open). It is important to note that **code repositories are not an appropriate way to distribute data**. ONS policies on security and all else can be found on [SharePoint](https://share.sp.ons.statistics.gov.uk/sites/knex/Policies/SitePages/Home.aspx).

Your work is covered by [Crown copyright](https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) - noting this and providing an appropriate license alongside your code is helpful to let others know how they can use, modify and redistribute your work. This is typically detailed as text in a LICENSE file. This [online tool](https://choosealicense.com/) might help you to choose an appropriate license for a given project, however, the Government Digital Service generally recommends using the [MIT license](https://opensource.org/licenses/MIT) for code and the [Open Government License (OGL)](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) for documentation.


## Getting started with GitHub

You should discuss the prospect of open sourcing with the head(s) of your team before getting started. If you have concerns or questions surrounding the topic, please look to online resources first but do feel free to get in touch for advice.
 
To get started, you'll need to register for a personal [GitHub](https://github.com/) account. You can use a personal email address for this, as your use of the platform might extend beyond your work at the ONS. However, you should still [add your ONS email address to the account](https://github.com/settings/emails) once it's created, to ensure that GitHub knows which account to assign your work to when working from an office machine.
 
<p align="center">
  <img src="https://github.githubassets.com/images/modules/logos_page/Octocat.png" alt="GitHub Octocat" width="20%" />
</p>
 
You can now follow these simple steps to [create](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github) and [clone](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-a-repository-using-the-command-line) a repository from GitHub. The courses on the [GitHub Learning Lab](https://lab.github.com/) are also great for walking through the basics. If you have any issues with Git or would like to modify your Git configuration further, I've put together a [guide on troubleshooting ONS Git configuration](https://github.com/best-practice-and-impact/ons-git-config) that you might find useful. Our team also have example projects for [Python](https://github.com/best-practice-and-impact/example-package-python) and [R](https://github.com/best-practice-and-impact/example-package-r) that you might find as a useful starting point.
 
Once you've created your own account, you are also able to create "[Organizations](https://docs.github.com/en/enterprise/2.19/admin/user-management/creating-organizations)" (I know, the z makes me sad too). Creating one of these for your team/division allows you to group open source code repositories together and easily collaborate on these projects internally and externally. Additionally, teams can be created, within these organization groups, to manage access to view or work on specific projects. 
 
It's worth noting that there is currently no centralised coordination of these organization groups at the ONS. You can, however, look towards owners of existing ONS GitHub Organizations for advice on creating one within your division/team, or perhaps associating your work with theirs:
* [Best Practice and Impact](https://github.com/best-practice-and-impact)
* [ONS Digital](https://github.com/ONSdigital)
* [Data Science Campus](https://github.com/datasciencecampus)
* [Big Data Team](https://github.com/ONSBigData) 
* [Sustainable Goals and Development](https://github.com/open-sdg)
* [Crime and Justice](https://github.com/ONS-centre-for-crime-and-justice)

If you're generally interested in contributing to or releasing your own open source software, you should also keep an eye out for next month’s [Hacktoberfest](https://hacktoberfest.digitalocean.com/). This international event points out plenty of resources on how to start contributing to open source and highlights beginner friendly issues across GitHub (plus you can get a free t-shirt and stickers!).

I hope that this article has been a useful introduction to versioning with Git, open source, and has started conversations around open sourcing your work using GitHub.
