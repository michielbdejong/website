# IndieHosters - Hosting for freedom, not for profit

## 1. Project plan

The project aims to build a network of independent free and open source Software-as-a-Service provider. The first goal is to define a standardized way of hosting a person's personal website and personal data server, based on existing free software products. It will allow experienced system administrators to start hosting these softwares - either for their own community, or as a single-person business. The second and main goal is to develop this network of independent hosters. We believe that local and small scale hosters are the way to fight against the ongoing gravitation of infrastructure and power to the "center" of the internet internet, e.g., google, facebook. And we believe it is the right time to do it, for two reasons:
- people are ever more aware of the need to redecentralize the internet
- automation tools start to be mature
It will allow us to build blazing simple tools, for powerful and resilient infrastructure.

### 1.1. the problem solved by this project

Let's say, there is a bug on Internet, e.g., gmail is spying on private conversations. Software engineers have power to resolve bugs. They write a piece of software, e.g., owncloud. People will install the source code on their server, bug solved! Most of people online don't even know what a server is and even less, what source code means. Did you realize that if you go to many FOSS project pages, you just have a `demo` possibility at best (e.g. Mailpile, yunohost) and a `download the source code` for the worsts. Why not having a classic `sign up` button? We propose to implement this sign up button. We will write a standardized install script to host all FOSS, and provide the service for the end user, in an easy way.

And, because we standardize the folder structure that contains the user data for each software application, people will be free to move between indiehosters by syncing their data folder to the new hoster. They will even be able to start their own server with their data. It is really important for us that people are free to change their service provider at any time.

###  1.2. the relative advantage of the proposed innovation

If you compare us to:
- google/facebook: our advantage is that we don't aim at selling personal data.
- wordpress.com: our advantage is that we will be much cheaper because we don't develop any software in-house.
- Yunohost/owncloud/cozycloud/sandstorm: our advantage is we will offer users any software they want, as long as it is free software we can host for them. Also, users will get the full package of indieweb identity, file server, and online applications, which existing providers do not do.

We aim local, and small scale, in the same way you trust more your local bio farmer than your supermarket.

###  1.3. usability: for whom and to what purpose

We firstly target a geek (woman or man). She/He is probably working as software engineer and cares about free software and likes playing around/tinkering with computers. And more generally, anybody that is concerned by privacy, and ready to give up a bit of usability and money in exchange of freedom. These persons are concerned by their privacy. And they want to take back control over their data. Unfortunately, these people don't have time or sufficient knowledge to administer these services by themselves.

###  1.4. perspectives for further development of this innovation and/or other technologies

As more and more people are concerned about their privacy and data ownership, we see more and more projects in this area trying to solve this issue. Most of them are software based, but without the service in mind. We see that more and more people are interested. So in terms of development, this is a really interesting area to focus on. And so the ultimate goal is for all people have their freedom box at home. In the mean time, as it is still complicated for most of the people, we offer them this hosted solution.

We believe that redecentralizing the internet is the most important mission we have today.

###  1.5. relevance for nlnet's mission

We believe writing software to make the internet a better place is nice. But it is not worth the effort if nobody is willing to host it. We offer to solve this challenge. Hosting Free and Open Source Software is the way to help people (not just geeks) escape mass surveillance, and getting back data ownership.

## 2. Existing work by others

The idea of a personal/cloud app store is not new. A lot of people already try to solve this challenge:
- freedom box
- yunohost
- cozy cloud
- sandstorm.io
- owncloud
- arkos

For now, just two of them offer hosting services as well (owncloud and sandstorm). The idea is to host them all, and offer the end user the choice for his app store (based on this existing list, and future software)

## 3. Existing work by us

We are at early stage of the project, and you can follow progress on our [GitHub account](https://github.com/indiehosters/). We already have static sites working with IPv6+SNI+SPDY, and an instance of yunohost. This allows us to provide emails and jabber for our end users.

## 4. Project setup

The project of bootstrapping the IndieHosters network will be entirely funded by donations and its goals are entirely non-profit. We aim to research, publish and educate. We publish everything under AGPL for software, and Creative Commons licenses for everything else. The project will employ [Michiel de Jong](http://www.linkedin.com/in/michielbdejong) and [Pierre Ozoux](http://www.linkedin.com/in/pierreozoux) as full-time free-lance contractor. Once the network is running in production, each indiehoster will bill his or her own users directly, possibly with a freemium or pay-what-you-like model.

Much of the expertise Michiel brings to the project, was built up as founder at unhosted.

Pierre works since two years as DevOps and software engineer for Seedrs. During this time, he contributed to some automation tools like Chef and Packer.

## 5. Project planning

We decided to quit our current position to start this project fulltime on the first of October. We are now in alpha phase with a bit less than ten alpha testers. We aim at reaching beta for first of january. Here is our planning, with deliverables, for the next two quarterly.

#### 1st January 2015: beta release
- a simple web app to provision users.
- a basic configuration for service provisioning tool (based on docker) to provide the following services
  - emails
  - jabber
  - static html
  - remoteStorage
  - sockethub
  - gitlab
  - openphoto
  - yunohost
  - owncloud
  - cozycloud
  - wordpress

At this stage users can ask us to manually perform the following actions
- start a service
- have a personal domain name
- backup personal data
- migration to another hoster

During the beta, most of the services are not yet automatic nor stables, but everything is working, even if it needs human intervention.

#### 1st April 2015: stable release

- control panel: a web app to control the following functionalities
  - start a service
    - linked to an advanced configuration for automatic service provisioning
  - configure domain name (with ssl certificate)
  - backup personal data
  - migration to another hoster

So the idea is to write two small pieces of software:
- a simple web application to allow users to manage their services
- a configuration to link this web application to a provisioning tool

We aim at simplicity, and writing as little code as possible. Just the strict necessary.

These two deliverables will be shipped the first of April (hopefully without jokes inside!).

## 6. Project budgeting

There is not much expenses besides the salary of the two founders. So the budget goes as following for the first six months:
The salary budget is 6x3000 = 18000 euros. This includes:

- 2000 euros/month net 'salary' - 2 people
- 300 euros/month German/Portuguese health insurance - 2 people
- 300 euros/month desk in a flex-office - 2 people
- 200 euros/month reserved for taxes and other administrative costs like registry and bank fees - 2 people
- 200 euros/month reserved for demo hosting, conference attendance, and miscellaneous costs - 2 people

There is also virtual machine cost. We aim at 10 euros/month/VM. We need two VMs per hoster. Which brings the total to 240 euros for six months.

The total budget is then 18240 euros.

It means that:
- beta release: 9120 euros
- stable release: 9120 euros

Two financing plans are thought:
- the perfect one: NLnet finances the beta and stable release.
- if it is not possible, we ask NLnet to kindly finance the beta, and we take care of financing the stable through crowdfunding and freelance.

In the latter case, the stable release would be delayed by at least one month (time to prepare crowdfunding campaign) if the crowdfunding is successful. Or many months in case we have to freelance to finish the project.

In any case, as the cost of the VMs is really low, we commit ourselves to keep running the services for the beta users.

## 7. Project risks

###  7.1. End users Adoption

The first risk is that we don't manage to convince people that our solution is better than YouNameIt SaaS. Most of people nowadays use proprietary SaaS and get used to their simplicity and integration. We know that our solution will be a bit more complicated and less integrated. At the beginning, it will be of course impossible to reach a user experience à la Apple. Plus, for long term sustainability, we aim at a donation based business model (like wikipedia) to finance salaries of hosters. It might be difficult to convince people to give money for a software they can have in exchange of their private data (which people value less and less).

To mitigate this risk we aim firstly at people aware of privacy issues on Internet. We hope this circle of early adopters will convince their circles, and little by little reach critical mass.

For the long term sustainability, we can also imagine all kind of hosters:
- for profit hosters (i.e. OVH, Gandi, 1and1)
- hosters reselling personal data (we are fine with that as long as the end user is aware)
- non-profit hosters (like us)

We find this way to be really healthy ecosystem. Then users will have choice among hosters. And if they want to pay with their private data, they'll also be free to do so. At least this is a closer definition of what we call an open and free (like in freedom) Internet.

###  7.2. Hosters Adoption

If not a lot of end users request this service, there will be no hosters (beside us) either. And this is also really bad. Bad in the sense that users will have the choice just between 2 hosters, us. This would be a limited definition of freedom to move your data.

We hope that by focusing on mitigating the first risk, this one will not happen.

## 8. Project results dissemination

Once we release the stable version, we have a creative way of disseminating the project. The idea is to replace the traditional `demo` button you can find on many FOSS projects by a `sign up` button. This button will bring the user to his personal hoster and allow him to use directly the software (without installing nor configuring any thing). The idea will be to work closely with FOSS developers to implement this functionality on the project page before they launch it in the media.

It will be a win/win partnership. FOSS developer will be happy because they will have more users using their software (so more people contributing to it). And we will be happy because we will have more users using our infrastructure (and at the end, more indiehosters).

## 9. Follow-ups on the project

This is a long term project. We ask NLnet help to bootstrap it, but we hope to be sustainable after stable release (thanks to donations). So the followup is as soon as it is stable, we add more and more services to our offer.

If we don't have anymore funding, that's also fine. If enough people are using it, more and more indiehosters will be there. So the community will be able to maintain the product by itself. And us, the founders, will continue to maintain our hosts and provide services (added by the community) to our users.
