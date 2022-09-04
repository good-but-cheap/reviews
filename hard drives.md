---
layout: review
title: Hard Drives
picture: /img/reviews/hdd.png
updated: August 2022
related:
    - USB-C-Laptop-Docks
    - cooler
---

{% capture considerations %}
- Form factor
- Capacity
- Speed
{% endcapture %}

{% capture know %}

### Form Factor
Hard drives come in a few different form factors, the first thing you need to know is [which kind you need](#Guide-to-identifying-the-Form-Factor-of-your-drive).
- The most common today are:
  - 2.5" or 3.5" SATA
  - M.2 NVMe
- For a computer that's a little older, it could also be:
  - mSATA (2013-2018, approx)
  - IDE (< 2000)
- For servers:
  - SAS

SATA drives come in two different sizes. 2.5" are common in laptops, and can also be used in desktops. 3.5“ drives are for desktops only. Occasionally laptops will have a constraint on the thickness of a SATA drive, but this is less common on recent drives and laptops.

SATA drives also come in two different types, solid state drives (SSD) and hard disk drives (HDD). SSDs are faster, but HDDs have larger maximum capacities and are cheaper per unit of storage space.

The speed difference is most notable when your computer is starting up, or when loading large applications, like games. 

If you're adding a drive, make sure you have a spare drive bay and connection available. If it's a replacement, make sure it will fit the replacement slot.
There's another common format it's almost definitely not what you need (unless you're a sysadmin for industrial servers), we mention it here only so it doesn't cause confusion, because they do turn up in search results occasionally.
SAS

### Capacity
Once you know the type of drive you need, you can start comparing different drives. The main considerations are capacity and speed.

The easiest way to judge the size you need, is to look at your current usage. See the guide below to check the size of your current drive, and how much of it is full. Then add some extra, because we always use more space, not less.

A note on units:
GB stands for Gigabyte, which is 1 billion bytes
A Terabyte (TB) is 1000 times bigger, 1 trillion bytes

The series of units is byte>kilobyte (KB)> megabyte (MB)> giga, tera, peta, …
You may also see other units for measuring data. Instead of gigabytes, you might see gibibytes, or gigabits. A gibibyte is about 7% larger than a gigabyte, a gigabit is about 12% the size of a gigabyte

1 TB is enough to cover most uses, and tends to be the current sweet spot in pricing, so we start our recommendations there.

### Speed

The best way to compare speeds is to look at the actual read and write speeds for specific drives. 
7 GB per second is about the fastest drive you will find today
Lower speeds, even below 100 MB per second are reasonable for some cases
Drives may have different read speeds and write speeds, in most cases, you write data once and read it many times, so read speeds should be prioritized

As general rules:
SSDs are faster than HDDs
M.2 NVMe is a faster interface than SATA
HDDs advertise the speed that the disks spin (7200rpm, 5400rpm, etc.), for disks of the same size (and with the same number of platters) these numbers are comparable, but a bigger disk will transfer data faster at a given spin rate, e.g. a 6TB drive at 5400rpm transfers data slightly faster than a 4TB drive at 7200rpm.

At Good But Cheap, we’re not above using bargain-brands, but hard drives are an item where it makes sense to stick to known brands. It’s easy to build a drive out of inferior parts and undercut on price, but those parts won’t last as long or perform as well. Stick with top brands like Wester Digital, Seagate, Samsung, Toshiba, and Crucial. The small premium is worth the increased reliability for your data.
{% endcapture %}

{% capture recommendation %}

## Some Good But Cheap Choices
|Model|Form Factor|Capacity|Link|Price|
|---|---|---|---|---|
|Seagate Barracuda Compute|3.5” SATA HDD|4TB|[Amazon](https://www.amazon.com/dp/B07D9C7SQH)|$68|
|PNY CS900|2.5” SATA SSD|1TB|[Amazon](https://www.amazon.com/dp/B07Y5VDNT9)|$63|
|Intel 660p|M.2 NVMe|1TB|[Amazon](https://www.amazon.com/dp/B07GCL6BR4)|$70|
{% endcapture %}

{% capture more %}
[PCPartPicker](https://pcpartpicker.com/products/internal-hard-drive/#sort=ppgb) has an excellent resource for finding hard drives. Sort the page by price per gigabyte, and then select filters for the type of drive you need.
Prices can change frequently based on supply and demand, and new releases. Though we list some good options here and update them often, a live tool is the best way to find a cheap drive that meets your needs.

## Guide to identifying the Form Factor of your drive:
![Drive Connectors](/img/reviews/hard-drives/connectors.jpg)
Current Drive Connectors. Left to right: 3.5" SATA, 2.5" SATA, and M.2 NVMe

![Older Drive Connectors](/img/reviews/hard-drives/legacy.jpg)
Some Legacy Drive Connectors: Left to right: IDE PATA, M.2 SATA

<div class="col-md-12 col-sm-12 portfolio-item">
  <a class="portfolio-link" href="/review/hard-drives">
    <img class="img-fluid" src="/img/reviews/hard-drives/connectors.jpg" alt="Current Drive Connectors">
  </a>
  <div class="portfolio-caption">
    <h4>Current Drive Connectors. Left to right: 3.5" SATA, 2.5" SATA, and M.2 NVMe</h4>
    <p class="text-muted"></p>
  </div>
</div>

<div class="col-md-12 col-sm-12 portfolio-item">
  <a class="portfolio-link" href="/review/hard-drives">
    <img class="img-fluid" src="/img/reviews/hard-drives/legacy.jpg" alt="Older Drive Connectors">
  </a>
  <div class="portfolio-caption">
    <h4>Some Legacy Drive Connectors: Left to right: IDE PATA, M.2 SATA</h4>
    <p class="text-muted"></p>
  </div>
</div>

## Guide to checking your current drive use:
- Windows
  - Open up "This PC" and each drive shows the space used and the total space on the drive.
- Mac
  - Open "About this Mac", then "Storage", then "Manage"
- Linux
  - Open "Other Locations" in the file browser, works on many distros -or-
  - Open a terminal and use the command $*df -hx tmpfs*

{% endcapture %}

{% include reviewtemplate.html %}