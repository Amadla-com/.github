<p align="center">
<img src="./assets/logo-big-circle.svg" alt="Amadla logo" width="400">
</p>

<h2>About</h2>

:warning: :construction: **Still in the works** :construction: :warning:

In the last decade, there has been a surge in tools designed to simplify the provisioning of cloud infrastructures, on-premise, and dedicated servers. While these tools offer significant benefits, setting them up and configuring them can be challenging, requiring considerable expertise in cloud systems, Infrastructure as Code (IaC), Linux, cybersecurity, and more. Many of these tools fall short of fully abstracting system-specific configurations, often necessitating detailed and complex setups.

For users who only need an environment to run a few server-side applications—like a VPN, blogs, email servers, or file managers—maintaining best practices and ensuring security can be daunting and time-consuming. Amadla aims to streamline this process by automating the setup of a basic environment suitable for personal use and businesses of all sizes. It simplifies the configuration of applications, servers, and cloud infrastructures by providing a solid abstraction layer.

<p align="center">
<img src="./assets/amadla-venn-diagram.svg" alt="Amadla Venn Diagram"/>
</p>

<h2>How Amadla Works?</h2>

Amadla uses a custom storage methodology called [HERY](https://github.com/AmadlaOrg/hery), which combines [YAML](https://en.wikipedia.org/wiki/YAML), [JSON-Schema](https://json-schema.org/), and [Git](https://git-scm.com/). This methodology provides a familiar yet innovative approach to configuration management. [HERY](https://github.com/AmadlaOrg/hery) extends [YAML](https://en.wikipedia.org/wiki/YAML) by grouping content into entities, similar to how an RDBMS (Relational Database Management System) organizes data. These entities can refer to other entities, with all content stored in text form, benefiting from [Git](https://git-scm.com/)'s version control capabilities.

The system also includes a caching layer based on [SQLite](https://www.sqlite.org/), enabling fast queries of configuration content. The [Amadla CLI](https://github.com/AmadlaOrg/amadla-cli) (Command Line Interface) queries [HERY](https://github.com/AmadlaOrg/hery) configurations and uses [Jinja2](https://jinja.palletsprojects.com/) templates to generate configuration files.

Each entity represents a block of mutable configuration standards. Users can create their own entities for any purpose or use the predefined ones provided by Amadla. Predefined entities ensure better integration with other tools and templates. For example, a "Net" entity attached to an application can specify the networking requirements for a website, inform the HTTP server, and configure the firewall to open the necessary ports. Configurations can be overridden in a cascading manner, allowing for flexible and hierarchical setups.

<!--<h2>Main Projects</h2>

<p>
 <a href="https://github.com/AmadlaOrg/amadla-cli"><img alt="Amadla CLI logo" src="./assets/amadla-cli-logo.svg" width="150" style="vertical-align: middle; float: left;"> amadla-cli</a> = <strong>Simple terminal application to use Amadla</strong>
</p>-->

<!--<p>
 <a href="https://github.com/AmadlaOrg/amadla-template"><img alt="Amadla Template logo" src="./assets/amadla-template-logo.svg" width="150" style="vertical-align: middle; float: left;"> amadla-template</a> = <strong>The Amadla template is a <a href="https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template" title="Creating a repository from a template">template</a> you can use to start with Amadla</strong>
</p>-->

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
