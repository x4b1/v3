<script setup>
    import jobLine from './job-line.vue';
    const jobs = [
    {
      title: 'Backend developer',
      start: '2020-07-27',
      end: '2021-07-28',
      company: 'Paack',
      website: 'https://paack.co/',
      logo: 'paack.png',
      description: [
        `Build new different backend services such as warehouse management system, drivers app.`,
        `Synchronizing services asynchronously with RabbitMQ and later with Pubsub.`,
        `Build APIs using Graphql.`,
        `Setup Helm charts and github actions for deployments`
      ],
    },
    {
      title: 'Software developer',
      start: '2018-11-13',
      end: '2020-07-24',
      company: 'Arex Markets',
      website: 'https://arex.io/',
      logo: 'arex.jpg',
      description: [
        `Created a service (front and back-end) to handle onboarding of the new customers, with different flows and external integrations, like contract
      generation, signing, notifications and other services.`,
        `Worked on developments around financial data, such as, invoice importing from third parties or financial transactions management.`,
        `Setup deployments, pubsub queues, and other infrastructure stuff.`,
      ],
    },
    {
      title: 'Backend developer',
      start: '2018-02-19',
      end: '2018-11-12',
      company: 'Holaluz',
      logo: 'holaluz.svg',
      website: 'https://www.holaluz.com/en/',
      description: [
        `Created from scratch a new managing tool for sales team. Build a service to handle automatically rejections from distributors when
      a customer wants to join.`,
        `Move legacy code to a new service cleaning the code and adding tests, also fix many bugs on legacy code.`,
        `Insfraestructure tasks, such as, create an ansible script to automatize the deployment of Nuxt static apps to Amazon S3.`,
      ],
    },
    {
      title: 'Squad leader',
      start: '2017-06-01',
      end: '2018-02-18',
      company: 'Inbenta',
      logo: 'inbenta.svg',
      website: 'https://www.inbenta.com/en/',
      description: [
        `Manage and develop a massive content importer from different sources, such as, Web (crawling), REST APIs, Zendesk, Salesforce, Shopify, Discourse... to automatically import contents to the company platform, allowing the client configure it selfs.`,
        `I was assigned the "Content Digest", a massive importer from different data sources, like, web crawling, Zendesk, Salesforce, Shopify. Also, I created a UI with Vue.js, allowing clients easily to set up his own importer.`,
      ],
    },
    {
      title: 'Full-stack developer',
      start: '2016-02-01',
      end: '2017-06-01',
      company: 'Inbenta',
      logo: 'inbenta.svg',
      website: 'https://www.inbenta.com/en/',
      description: [
        `Manage projects related to chat-bots, NLP search and ticketing. Talking with clients to analyse the needs and viability.`,
        `Develop functionalities for customer adapting company product to each them.`,
      ],
    },
    {
      title: 'Developer Intern',
      start: '2014-10-01',
      end: '2016-02-01',
      company: 'Arin Innovation',
      logo: 'arin.jpg',
      website: 'http://www.arin-innovation.com/en/',
      description: [
        `I did my first internship at Arin Innovation, a consulting services company.`,
        `My daily work was to talk with clients to get the requirements and develop them. There I learned to apply the knowledge learned to develop with Oracles tools, such as JD Edwards and Oracle DB.`,
        `First I was contracted for one year, when it finished they proposed me to extend the contract.`,
      ],
    }]
</script>
<template>
<div>
    <h3 class="font-medium leading-tight text-3xl mt-0 mb-2">Experience</h3>
    <job-line v-for="job in jobs" :key="job.company" :job="job" />
    </div>
</template>
