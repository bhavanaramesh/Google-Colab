**Google Colab Tutorial**
Colab is a Google’s free cloud service which will let you run your deep learning or machine learning models in cloud.

**Creating New Colab Notebook**
Open your Google Drive

**Create a new notebook via Right click > More > Colaboratory**

**GPU Setting**
Edit > Notebook settings or Runtime>Change runtime type and select GPU as Hardware accelerator

**RAM Info**
>!cat /proc/meminfo

**CPU Info**
>!cat /proc/cpuinfo

**Install Libraries**
>!pip install or !apt-get install

>!pip3 install tensorflow==1.8
>!pip3 install keras
>!pip3 install torch torchvision
>!apt-get install python-numpy python-scipy



**Cloning Github Repo to Google Colab**
>!git clone https://github.com/ildoonet/tf-pose-estimation.git

**Mount your Google Drive**
>from google.colab import drive
>drive.mount('/content/drive/')

**Check your Folder Data**
>!ls Drive/test

**Upload code from your system**
>from google.colab import files
>uploaded = files.upload()

**Make zip file of your Data**
>from google.colab import files
>import zipfile
>import sys
>foldername = 'your folder or filename'
>zipfile.ZipFile('Drive/'+foldername + '.zip', 'w', zipfile.ZIP_DEFLATED)


**Downloading the data from the colab**
>from google.colab import files
>files.download('Drive/test.zip')
