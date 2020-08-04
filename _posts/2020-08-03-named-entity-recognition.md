# Why Your Company Should Care About Named Entity Recognition

![](/images/2020-08-03-named-entity-recognition/media/image1.jpeg)source: [<span class="underline">PhotoMIX Company</span>](https://www.pexels.com/@wdnet) from [<span class="underline">Pexels</span>](https://www.pexels.com/photo/vegetables-stall-868110/) (CC0).

Named entity recognition is the task of categorizing text into entities, such as people, locations, and dates. For example, for the the sentence, On April 30, 1789, George Washington was inaugurated as the first president of the United States , this sentence may be tagged with the following entities:

![](/images/2020-08-03-named-entity-recognition/media/image2.png)

You might be thinking, okay exactly how is this useful? Well, there are many potential uses of named entity recognition, but one is being able to make a database easily searchable. You might be thinking, why would I need to tag entities to make a database easily searchable? Can’t I just use a simple dictionary lookup to exactly match terms? Well, yes, you can, but this is far from ideal and just to show you how ineffective searches can be without named entity recognition, let’s walk through a real life example.

## Example

Recently I was ordering food at my local grocery store, [<span class="underline">Weis Markets</span>](https://www.weismarkets.com/), and was trying to add to my cart Perdue frozen chicken fingers. So I typed into the search bar:

![](/images/2020-08-03-named-entity-recognition/media/image3.png)

To my disappointment, my search did not yield any results:

![](/images/2020-08-03-named-entity-recognition/media/image4.png)

At first I thought they may have been out of stock, but after searching for several other items, I kept getting no results. After awhile, I started to suspect that Weis’s search engine was only able to find search terms that almost exactly matched the product label (Note: I do not actually know the machinery behind Weis’s search engine). So I looked up on Google what the chicken fingers I wanted were exactly called and I realized they are called chicken *tenders* not *fingers* (of course!). So I typed perdue chicken tenders into the search box and it worked! I was then successfully able to add the chicken fingers to my cart.

![](/images/2020-08-03-named-entity-recognition/media/image5.png)![](/images/2020-08-03-named-entity-recognition/media/image6.png)

I was happy that I was able to add the chicken fingers to my cart, but this was a lot of work to just find one item and I had this same issue with several other items. This made Weis’s online shopping almost unusable! Since then I have not purchased groceries online from this store — it’s just too much work.

## The Solution

Fortunately for Weis Market, there is a somewhat easy fix to their search engine issue and that is to use named entity recognition. With named entity recognition, the search engine should automatically tag each of the entities. For example, when I typed in perdue chicken fingers it should have tagged Perdue as the brand and chicken fingers as chicken tender (I am not not an expert in food categories, so I do not actually know if chicken tender would be a useful category).

![](/images/2020-08-03-named-entity-recognition/media/image7.png)

Then, this would search through a database, where each item has been previously tagged. So the actual chicken fingers I wanted may have been previously tagged with the following categories: **brand**=Perdue; **food**=chicken tender; **frozen, fresh, canned**: frozen.

![](/images/2020-08-03-named-entity-recognition/media/image8.png)

With the use of these entities and a structured database, my search for perdue chicken fingers would have matched Perdue as the brand and chicken tender as the food and would likely have included the chicken fingers I wanted in my search results.

## Conclusions

So as you can see, named entity recognition can be extremely useful and is almost essential for some products. You can imagine all the possible other uses besides creating a search engine for a grocery store (e.g., recommending similar online articles based upon tagged entities, creating an easily searchable database of interview transcripts, etc.). Something I have not mentioned in this post is the machine learning approaches that may be used to actually conduct the named entity recognition task (in the example, the task of tagging entities in the search perdue chicken fingers). This is the first installment of a series of blog posts about named entity recognition and the next post will go more into the technical details. Lastly, if you think your company may benefit from named entity recognition, feel free to reach out to me — my contact information may be found on my [<span class="underline">website</span>](https://zachmonge.github.io/).