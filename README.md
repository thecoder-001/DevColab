<h1 align="center">DevColab</h1>
<p align="center">A development environment in Google Colab</p>
 <a href="https://colab.research.google.com/github/thecoder-001/DevColab/blob/master/DevColab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" align="right"></a>

## :hear_no_evil:  First of all, what is google Colab?
As the official FAQ says, colaboratory, or “Colab” for short, is a product from Google Research. Colab allows anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs.
In short, it is a vm provided for learning, running python code, machine learning or for general purpose.

## :moneybag:  Is it really free to use?
Yes, Colab is free to use. But there are some points which, according to me one should keep in mind:
1. Though colab is a free service, it shouldn't be exploited indiscriminately or without any care. One should value that its a resource offered for no cost and can get depleted/restricted if the demand increases out of control.
2. If it isn't obvious, one shouldn't run mission-critical services (like large and important servers/databases/python programs) on it. Its resources are not guaranteed and not unlimited, and the usage limits sometimes fluctuate. Also, the notebook has a maximum runtime of 12 hours, after which, it should be manually restarted.
3. One should not try to spread it as wildfire (in my opinion), that there's a free service available to every living being out there. If such a sudden boom in user base happens, Google would be forced to close down the free teir of google colab, devoiding many hobbists of the free service. Keep it like a secret, telling it to only those who are worthy and know how to use it.

Blah blah blah...its a private repo so not much matters. Use it freely as you wish but keep point 3 in mind.

## :zap:  So, how does it actually work?
As Google Colab is a VM running Ubuntu server as base OS, it can be easily used as a remote development enviornment. Here are the steps which the notebook performs to setup the server:
1. Update the system's apt cache.
2. Upgrade the system's packages.
3. Mount Google Drive to access the files (Drive is used here to provide persistent storage).
4. Setup Ngrok (by asking for key by user).
5. Install and setup code-server to facilitate VScode in browser.
6. Startup the VScode server (with defined config and working directory in google drive) <br>
   \[or] Startup ssh server.
