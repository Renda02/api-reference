# Using Nexthink Assist

Nexthink Assist is the unified entry point to managing digital employee experience across the entire Infinity platform. Embedded directly into the search navigation, Nexthink Assist uses the latest large language models from OpenAI and Anthropic to help IT teams see, diagnose and fix DEX challenges instantly through the power of Generative AI. In particular, Nexthink Assist enables users to perform contextual searches across product documentation, extract data on device performance, user sessions, and applications, and quickly create Nexthink campaigns using natural language requests.

<figure><img src="../../.gitbook/assets/AboutAssist.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Nexthink Assist is currently in **Beta** and is continually improving. As it evolves, it may occasionally provide information that requires verification. Nexthink recommends confirming your results to ensure accuracy while using Nexthink Assist.
{% endhint %}

## Getting started with Nexthink Assist <a href="#how-to-get-started-with-assist" id="how-to-get-started-with-assist"></a>

First, ensure that your role allows you to view Nexthink Assist**.** Refer to the [Permissions](./#permissions) section for more information.&#x20;

To access Nexthink Assist, select **Nexthink** **Assist** from the main menu.

<figure><img src="../../.gitbook/assets/Assist - 1721048792.png" alt=""><figcaption></figcaption></figure>

The Nexthink Assist window appears, allowing you to type your text into the search bar. Use the following options to get the information you need:

* **Search**: Type text in the search bar **without hitting Enter** to conduct searches across various parameters. Refer to the [Using Search](https://docs.nexthink.com/platform/user-guide/search-and-nexthink-assist/using-search) documentation for more information.&#x20;
* **Assist**: Type text in the search bar and **hit Enter** to create investigations and campaigns, or to get answers related to Nexthink Infinity.

<figure><img src="../../.gitbook/assets/Assist - 1721114015.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Type at least **3 words** and press the **Enter** key to activate **Assist**. To continue using **Search** in standard mode, type the name of a binary, device, or package.
{% endhint %}

Use Nexthink Assist to simplify building investigations, streamline campaign creation, and answer your questions about Nexthink Infinity.

* **Ask about Nexthink**: Assist enables contextual search across product documentation to get you started quickly, with the information and context you need.
* **Query Data**: Assist helps you extract data and quickly find answers about device performance, binaries, user and session data, application information, and more to resolve issues proactively.
* **Create**: Assist helps you create Nexthink campaigns, making campaign building instantaneous. Compose a quick request in natural language, and watch Nexthink do the rest.

In addition to its three main capabilities, Assist answers your questions across all Nexthink Infinity configuration objects available in your environment. Use Assist to get answers about live dashboards, monitors, library packs, and more.

<figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

Once you send your question to Assist, it generates and executes an NQL query, creates a campaign or provides an answer from the documentation.&#x20;

Ask follow-up questions on the same topic to keep the current conversation going. To start a conversation from scratch, click the reset button in the top-right corner of the Nexthink Assist window.&#x20;

<figure><img src="../../.gitbook/assets/Assist - 1723097609.png" alt=""><figcaption></figcaption></figure>

Imagine that you work for a company with a Sales department in Boston. This department has complained about problems with MS Teams call quality. You decide to investigate this issue using Nexthink Assist. The following documentation sections provide guidelines on using Nexthink Assist with examples related to this use case.

## Query data with Assist

To identify the cause of the MS Teams call quality issue, ask Assist to _display the average Wi-Fi signal strength per US city sorted in ascending order_ and **hit Enter**. The query that Assist creates immediately reveals that the Boston office has the worst Wi-Fi signal strength.

<figure><img src="../../.gitbook/assets/Assist - 1723097426.png" alt=""><figcaption></figcaption></figure>

Continue the conversation with Assist in the same window and ask for a _list of Sales department employees in Boston_. Then, click on **View in Investigations** to access the **Investigations** module and get the full list. Refer to the [Visual editor](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/visual-editor) and [NQL editor](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/nql-editor) documentation for more information about Investigations.

<figure><img src="../../.gitbook/assets/Assist - 1723097541.png" alt=""><figcaption></figcaption></figure>

### **Data out of Assist scope**

[Nexthink NQL data model](../nexthink-query-language-nql/nql-data-model.md) provides an overview of the data Nexthink collects. Assist currently supports most of the NQL data model, **excluding** custom fields and the below list of fields**:**

| Namespace          | Unsupported tables                                                                                                     |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------- |
| application        | network\_application                                                                                                   |
| alert              | impact                                                                                                                 |
| device             | device/local\_admins                                                                                                   |
| remote\_action     | execution\_summary                                                                                                     |
| service            | all                                                                                                                    |
| software\_metering | all                                                                                                                    |
| connection         | <p>udp_event<br>tcp_event</p>                                                                                          |
| session            | <p>connect<br>disconnect<br>lifecycle_event<br>lock<br>logout<br>unlock</p>                                            |
| web                | <p>error_summary<br>event_summary<br>transaction_summary<br>page_view_summary<br>page_view/detailed_page_load_time</p> |
| workflow           | execution\_summary                                                                                                     |

{% hint style="info" %}
The response times of Assist may vary, and occasionally, some Assist-generated queries might not display correctly in the [Visual editor](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/visual-editor).
{% endhint %}

## Create campaigns with Assist

Once you have identified the problem with the Wi-Fi signal strength in the Boston office, the next step is notifying all affected employees via a Nexthink campaign.&#x20;

Use Assist to _create a campaign to inform employees that the Boston office has Wi-Fi issues._ Assist creates this campaign—questions and answers—according to your instructions.

<figure><img src="../../.gitbook/assets/Assist - 1723097717.png" alt=""><figcaption></figcaption></figure>

If you would like to improve your campaign, type additional commands into the search bar to provide further guidance.&#x20;

<figure><img src="../../.gitbook/assets/Assist - 1723196848.png" alt=""><figcaption></figcaption></figure>

If you are satisfied with the suggested campaign, simply type **Yes** in the search bar to save it as a draft in the **Campaigns** module and define targeted users and the trigger mechanism. Refer to the [Creating Campaigns](https://docs.nexthink.com/platform/user-guide/campaigns/creating-campaigns) documentation for more information on how to finalize a campaign draft and distribute it among selected audiences.&#x20;

### Types of campaigns Assist can create <a href="#what-type-of-questions-can-assist-answer" id="what-type-of-questions-can-assist-answer"></a>

Assist can help you complete the content section for any [type of Nexthink campaign](https://docs.nexthink.com/platform/user-guide/campaigns/creating-campaigns/types-of-campaigns). Examples:

* _Create a device usage survey_
* _Create a campaign to inform users about ongoing Wi-Fi issues in our office_
* _Create an IT satisfaction survey_

Refer to the [Conducting engaging campaigns](https://docs.nexthink.com/platform/user-guide/campaigns/getting-started-with-campaigns/conducting-engaging-campaigns) documentation for more information about creating effective campaigns.&#x20;

## Ask Assist about Nexthink Infinity

Wi-Fi problems are very common and can occur again. Use one of the monitors available in Nexthink Library to effectively monitor Wi-Fi issues and take action to resolve the issue. Ask Assist how you can enable the monitor in the Alerts module.&#x20;

<figure><img src="../../.gitbook/assets/Assist - 1723204902.png" alt=""><figcaption></figcaption></figure>

Assist uses Nexthink Infinity documentation resources to provide the best answer. For further information or instructions, refer to the relevant documentation pages and training linked by Assist at the bottom of its response.

### Types of questions Assist can answer <a href="#what-type-of-questions-can-assist-answer" id="what-type-of-questions-can-assist-answer"></a>

Assist answers your questions using Nexthink Infinity documentation, which includes in-product, and online documentation sources.&#x20;

Question examples:

* _How to configure a webhook?_
* _What is the difference between hard and soft navigations?_&#x20;
* _What is the limit of campaigns I can create in Workplace Experience?_&#x20;

## Frequently Asked Questions <a href="#title-text" id="title-text"></a>

<details>

<summary>I'm getting unexpected answers from Assist. What can I do?</summary>

It may be that the answer to your question is based on a topic Nexthink Assist does not support. Refer to the [What type of Investigations can Assist create?](using-nexthink-assist.md#what-type-of-investigations-can-assist-create) section for more details.

Assist uses natural language to answer your questions. Sometimes, you might observe that Assist cannot respond to your question or that the response is incorrect. Here are some recommendations for how you can best phrase your questions:

* **Be clear and specific**: Provide clear information about the issue you are investigating. Avoid vague or ambiguous questions that may lead to inaccurate results.
* **Use targeted keywords**: Use relevant keywords related to the problem you are trying to solve whenever possible. This helps Assist in understanding the context and providing more accurate responses.
* **Frame your questions**: Structure your prompts as questions or specific commands. For example, instead of typing _Find errors in Teams_, try _How many Teams calls had bad quality in the last 24 hours?_
* **Experiment and iterate**: If you do not get the desired results initially, don't hesitate to refine your prompts. Assist learns and improves over time, so experimenting with different phrasing can help you achieve better outcomes.

For more information on effective prompt writing, complete the online course [_How to fast-track work with Nexthink Assist_](https://learn.nexthink.com/courses/how-to-fast-track-work-with-nexthink-assist) available on Nexthink Learn.

</details>

<details>

<summary>How can I share feedback on Assist with the Nexthink team?</summary>

Help us improve Assist by sharing your feedback using the thumbs-up and thumbs-down icons located in the lower-right corner of the latest response from Assist.


<summary>As Nexthink admin, can I pilot the usage of Assist before exposing it to a broader user group?</summary>

Yes, Nexthink admins can pilot the usage of Assist by selectively disabling and enabling the Assist permissions of certain roles.&#x20;

</details>

<details>

<summary>Does Assist apply View-domain constraints and permissions?</summary>

Yes, the View domain applies to Assist. For example, Nexthink users querying data with Assist will get the same results as running the query in NQL or the Visual editor.&#x20;

Nexthink also enforces permissions before performing a task. For example, to view and use the **Create** campaigns feature in Nexthink Assist, ensure that your role has permission to _edit campaigns_. Without this permission, you cannot create campaigns and will receive the following error message: _You do not have the right permissions to perform this action. Please reach out to your administrator._&#x20;

</details>

<details>

<summary>Is Nexthink Assist an add-on product? Does it require an additional license?</summary>

Nexthink Assist is an Infinity feature, part of the Workplace Experience core product, and available at no additional charge.

</details>
