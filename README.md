# Particle Integration

## In ilert: Create a Particle alert source

1. Got to **Alert sources** -> **Alert sources** and click on **Create new alert source**

![ilert alert source 1][1]

2. Search for **Particle** in the search field, click on the Particle tile and click on **Next**.

![ilert alert source 2][2]

3. Give your alert source a name, optionally assign teams and click **Next**.
4. Select an **escalation policy** by creating a new one or assigning an existing one.

![ilert alert source 3][3]

5. Select you Alert grouping preference and click **Continue setup**. You may click **Do not group alerts** for now and change it later.

![ilert alert source 4][4]

6. The next page show additional settings such as customer alert templates or notification prioritiy. Click on **Finish setup** for now.
7. On the final page, an API key and / or webhook URL will be generated that you will need later in this guide.

![ilert alert source 5][5]

## In Particle: Create a Webhook

1. In the sidebar click on **Integrations**.

![particle webhook 1][6]

2. Now click on **ADD NEW INTEGRATION**.

![particle webhook 2][7]

3. Click on **Webhook**, to create a new webhook integration.

![particle webhook 3][8]

4. Enter a **Name**, an **Event Name**(ALERT or RESOLVE) and the previous generated ilert webhook URL into the **URL** field.
5. Change the **Request Type** to **POST** and open the **Advanced Settings**.

| ALERT  | RESOLVE |
| ------------- | ------------- |
| ![particle webhook 4][9]  | ![particle webhook 5][10]  |

6. Select **Default**. (for custom json data follow this step)

![particle webhook 6][11]

7. Click on **SAVE**.
8. Optional: Click on **TEST** to test the integration.

![particle webhook 7][12]


## Custom Webhooks

### In Particle: Custom json data

1. Under Advanced Settings choose **Custom** for **JSON DATA**.
2. Create a template using the [Particle documentation](https://docs.particle.io/reference/cloud-apis/webhooks/). (it is also possible to add own customized values)

![particle webhook 8][13]

### In ilert: Create a custom template

1. Go to the alert source edit view.
2. Under **Alert template** enable **Alert summary** and **Alert details**.
3. For a detailed guide on how to use our alert templating click [here](https://docs.ilert.com/alerting/alert-sources#customize-your-alerts-with-alert-templates).
4. Use the payload keys created in Particle to create the alert template.

![particle webhook 9][14]

[1]: https://github.com/iLert/particle-integration-docs/blob/master/images/ilert_particle_1.png
[2]: https://github.com/iLert/particle-integration-docs/blob/master/images/ilert_particle_2.png
[3]: https://github.com/iLert/particle-integration-docs/blob/master/images/ilert_particle_3.png
[4]: https://github.com/iLert/particle-integration-docs/blob/master/images/ilert_particle_4.png
[5]: https://github.com/iLert/particle-integration-docs/blob/master/images/ilert_particle_5.png
[6]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_1.png
[7]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_2.png
[8]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_3.png
[9]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_4.png
[10]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_5.png
[11]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_6.png
[12]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_7.png
[13]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_8.png
[14]: https://github.com/iLert/particle-integration-docs/blob/master/images/particle_ilert_9.png
