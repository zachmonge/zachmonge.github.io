# A Data Scientist’s Guide to Creating and Deploying Apps

## A quick guide for data scientists on resources for creating and deploying web applications.

![](/images/2021-07-11-create-deploy-apps/media/image1.jpeg)source: [Nina Uhlíková](https://www.pexels.com/@ninauhlikova) from [Pexels](https://www.pexels.com/photo/person-standing-on-hand-rails-with-arms-wide-open-facing-the-mountains-and-clouds-725255/) (CCO).

I am frequently asked by other data scientists and students the best way to create and deploy apps. And creating apps is a great idea! It is very powerful to be able to deliver a machine learning project in some type of interactive format. However, as data scientists, we typically are not experts in web development, so, historically, we had to collaborate with web developers to create apps (not that there is anything wrong with that and there are still many times where we may want the experts come in to create our apps). Well in 2021, thanks to many open-source developers, data scientists are empowered to make their own apps without spending an excessive amount of time studying web development! Creating apps for data science projects is easier than ever. Here, I share a couple of libraries and resources I have found useful.

## But Don’t We Already Have Software for Creating Dashboards?

Before going into the technical details, at this point, if you are a data scientist, you might be wondering why am I saying we have never been able to create apps where data scientists for over a decade have been deploying dashboards. That is completely true! There are many cases where dashboard software, such as Tableau, are completely appropriate and sufficient for a project. However, there are times where they can be limiting. For example, let’s say you want to deploy a machine learning model. I have never used dashboard software such as Tableau, but from what I can tell, if you want to deploy a machine learning model in your dashboard, this would extremely difficult if not impossible. That’s where apps come in. They offer data scientists a lot more flexibility to build what they want!

Now that we are all convinced that creating apps is a powerful skill, let’s go more into the technical details.

## Python vs. R

Here is the cool part about app libraries designed for data scientists, many of them are in languages we use on a daily basis, such as Python and R!

For what software to use to create apps, it will depend on what coding language you are most comfortable writing — here, I am referring to Python vs. R. In terms of which programming language is better, there are pros and cons to both languages, but I always recommend to students to learn Python because of the large number of data science packages available in Python and, depending on the company (there is variability!), when you have a job in industry, your team is likely to be more familiar with Python (there are several other reasons why I prefer Python but I will not go into detail here). But if you are more familiar with R, the best app library for you probably will be [Shiny](https://shiny.rstudio.com/). With that being said, I have never used Shiny so I cannot say much about it, but it is extremely popular among R users.

For Python users (**the recommended approach**), I strongly recommend [Streamlit](https://streamlit.io/). Streamlit is extremely easy to learn (they have a great tutorial [here](https://docs.streamlit.io/en/stable/tutorial/create_a_data_explorer_app.html)). The only prerequisite for using Streamlit, is having some familiarity with Python — if you are interested in learning Python, I wrote another blog post about it which can be found [here](https://towardsdatascience.com/learning-to-code-for-data-scientists-and-academics-8019b4677537).

## App Deployment

Now that you know how to create an app with Streamlit, the next step is deploying your app. The approach you take for deployment will depend on (1) privacy restrictions and (2) the complexity of the app.

### Streamlit Sharing

![](/images/2021-07-11-create-deploy-apps/media/image2.png)source: [Streamlit](https://streamlit.io/brand)

If you are able to make your code and app publicly available, one easy way to deploy your app is directly through [Streamlit sharing](https://docs.streamlit.io/en/stable/deploy_streamlit_app.html). I have never actually used Streamlit sharing before, but from skimming the documentation, it sounds relatively easy. However, I believe you are only able to share a limited number of apps.

### Docker and Cloud Service

![](/images/2021-07-11-create-deploy-apps/media/image3.png)source: [Docker](https://www.docker.com/company/newsroom/media-resources)

Another option is to wrap your Streamlit app into a [Docker](https://www.docker.com/) container (if you have never heard of Docker, check out this [blog post](https://towardsdatascience.com/how-docker-can-help-you-become-a-more-effective-data-scientist-7fc048ef91d5)) and deploy your container on some cloud service, such as AWS. [Here](https://maelfabien.github.io/project/Streamlit/#dockerfile), is a blog post that explains how to do this with a relatively simple app. Depending on the machine learning model contained in your app (if any), how many users will use your app, and if you need feedback from the users, app deployment can quickly become complicated. Luckily, cloud services such as AWS and GCP provide services that can help in these scenarios but it does take some work to become comfortable with these services. There is actually a really good tutorial that clearly walks through some of these complexities, which can be found [here](https://www.mrdbourke.com/cs329s-machine-learning-deployment-tutorial/).

### Company Specific Deployment Services & Other Services

Lastly, the company you work at may have some other type of deployment service, which could possibly be used to deploy a Streamlit app. It’s, of course, worth checking out these options if they are available.

## Conclusion

As can be seen from this blog post, creating and deploying apps is relatively easy (well, for the most part!), which makes this a really exciting time to be a data scientist! I hope you find this post useful and happy coding!
