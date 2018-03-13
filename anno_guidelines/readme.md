# Manual annotation of the parallel data

* Step 1. Retrieval of relevant data from the parallel corpus files.  
* Step 2. Data preprocessing and encoding.  
* Step 3. Dependency annotation (using UDpipe).  
* Step 4. Data post-processing.  
* Step 5. 1-4 with parallel data (Russian data) and word-by-word alignment.  
* Step 6. Editing POS tags, lemmata and grammatical information.  
* Step 7. Editing syntactic relations (using Annotatrix).  

## Step 1. Retrieval of relevant data from the parallel corpus files.  
The RNC parallel corpus data have the following xml representation. We can collect data for each language using the following commands. 
In Linux/MacOS Terminal:
```
cat *.xml | grep 'lang="be"' > output.txt
```

Using Windows PowerShell:
```

```


## Step 2. Data preprocessing and encoding.  
We will keep information about location of each paragraph in the parallel corpus files in order to simplify the alignment. WE will keep information about tokenization and sentence boundaries, if available. However, this information can be misinterpreted by UDpipe (see Step 3), so the idea is to screen it from the parser as much as possible.  

### Parallel corpus files and lines info  

### Strings split problem (optional)
Windows PowerShell tends to split the paragraph strings at ca. 80 characters. If so...
In NotePad++
```
Find:

Replace: 

Find:

Replace:

```

### Full stops split
```
# Find:
^(\d+\t[^\t.]+)\.
#Replace
\1\3\n\t\2
```


## Step 3. Dependency annotation (using UDpipe).  
**UPpipe** online service is available [here](https://maryszmary.github.io/ud-annotatrix/standalone/annotator.html). Experienced users can also download and run UDpipe from a command line as described [here](http://wiki.apertium.org/wiki/UDPipe).

## Step 4. Data post-processing.  


## Step 5. 1-4 with parallel data (Russian data) and word-by-word alignment.  


## Step 6. Editing POS tags, lemmata and grammatical information.  


## Step 7. Editing syntactic relations (using Annotatrix).  
**Annotatrix** can be found [here](https://maryszmary.github.io/ud-annotatrix/standalone/annotator.html). Please contact Maria Sheyanova in case you have any questions.

