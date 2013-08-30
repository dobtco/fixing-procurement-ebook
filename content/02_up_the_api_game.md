## How To Fix Procurement #2: Up The API Game

We're dedicating this week to talking about how to fix procurement. Yesterday we discussed [where to start in procurement reform](http://blog.dobt.co/Fixing-Procurement-1-Fix-Registration/) -- fixing the registration process for businesses -- and today we're going to provide an example of one way to fix it: by upping the government's API game.

<!-- more -->

To date, government APIs have largely been discussed as a method for expressing data to citizens. It stems from the open government's roots in the transparency movement -- that government data ought to be free, so that it can be more transparent and effective. Though most of the time, it's the case that developers (who are really the only people who can use APIs) most government data doesn't really require an API as much as it requires a well thought out, well formatted, and well maintained .csv file. Rarely does government data require cloud based computational capacity to add value to the raw data, and rarely does it grow so big that an API becomes more useful than managing the data locally gets unwieldy.

We need to start thinking about APIs, instead, as a method for improving the user experience of government. The registration process is a great place to start, because it's a confusing area that's rife with awkward user interfaces. Imagine, instead, if when you file for incorporation with LegalZoom, you're asked to certify that you're a woman-owned business and it instantly registers you with the SBA as such for an extra fee. Or that QuickBooks notices that you fall below the small business threshold for your given industry, and asks you if you'd like to self-certify for a fee?

If business registration entities like the GSA, the SBA, or local business development organizations create APIs around their registration processes they can leverage the private sector to compete to see who can make it the easiest and cheapest to register these businesses for working with government at the federal state and local level.

Moreover, as long as government has provided registration free of cost via its own website, it can justify charging for API access and create a revenue opportunity for itself. It's not charging people for something taxpayers are already paying for -- it's charging businesses to enhance their existing products. Charging a nominal amount for access to this API is probably a good API to fight fraud and prevent spam, and would likely be one that the Intuits and LegalZooms of the world would gladly pass on, and probably keep the API revenue neutral. This opens the door to ethical revenue based contracting: I'd happily build an API on top of Sam.gov's registration process for free, in order to get $1 every time someone uses that API to register a new entity.

The one trick is to make it easy to sign up for API access. We don't want to just shift the registration burden from citizens to developers, we also want developers to be able to register easily.  The IRS's leadership in the sector with the E-Filling API -- the one that empowers companies like TurboTax -- is a [good place to start](http://www.irs.gov/Tax-Professionals/e-File-Providers-&-Partners/Become-an-Authorized-e-file-Provider#phase3), but the barrier still likely needs to be dialed back for things less universal than paying taxes. Usually charging a small fee per-request will filter out more fraud than stringent background check requirements.

In general, government needs more process focused APIs. Everywhere there's a government form, there's a case for an API, and a business ecosystem to be built on top of it. Obviously some business cases (like tax filing) are more viable than others (like Race To the Top application forms). A way to prioritize this list is using a little known system called the [ICR Dashboard](http://www.reginfo.gov/public/jsp/PRA/praDashboard.jsp). The federal government has to calculate the number of "burden hours" it takes to fill out the form. The formula is simple: number of respondents times the time it takes to fill out. This system has a list of all the forms, and all the burden hour estimates.

Opportunities exist when there are high numbers of burden hours, or solely a high number of respondents. It's unfortunate that the agency that runs this site, [OIRA](http://www.whitehouse.gov/omb/inforeg_administrator) doesn't provide a list of all the government forms ranked by these numbers. They do, however, provide an [xml dump of all government's forms](http://www.whitehouse.gov/omb/inforeg_xmlreports). That's a good list of where to start. And interestingly, leveraging an API first strategy may allow federal programs to avoid some [paperwork reduction act](http://www.informationdiet.com/blog/read/the-law-everyone-should-hate) issues (for instance, a private entity can engage in multivariate testing of a form, the federal government, ridiculously, cannot), since a private entity is actually doing the information collection.

The interesting thing about this opportunity is that for many of these is that if you don't work for government, there's still an opportunity for you. One needn't wait for government to make an API. Often, you just need to understand what the form is trying to accomplish, who its customers are, and how to certify it and send it in to government.

We at the Department believe there ought to be more players in this space. So we took the XML dump, and turned it into a [Google Spreadsheet](https://docs.google.com/spreadsheet/ccc?key=0AsUDSmA6u13VdEk0SXYxeEUtajlyTXBESU1oQUR3TVE#gid=0). Want to see which government forms take the most time and thus have the most opportunity? Now you can.