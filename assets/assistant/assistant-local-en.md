# Add Local Dataset 

You can add your own local file to this assistant and chat with your own data. You can add mulitple files to this assistant, and chat with these files.
Also, you can remove any file at any time you want to delete memory of this assistant without any effect on any other files/memories.
The total files you can uploaded is limited by your subscription plan.


### Add local file
1.  Click the avatar button in the right up corner of top navigation bar, in drop down menus, select My Assistants
2.  In your assistant dashboard, click the assistant name to navigate to assistant detail page.
3.  Click Dataset menu on left section, you can see the files learned by this assistant.
4.  Click 'Add dataset' button, Click Local tab
5.  On Local tab, click attach file icon in input field, select your local file to be learned.

> Note: file types supported:
> + PDF(.pdf)
> + Txt(.txt)
> + Word(.doc/.docx)
>
> Your local file should have these file extentions included, otherwise an error will be occoured.

6.  Click Upload button to start upload, when upload finished, the trainning will start automatically.
7.  Checkout the trainning status by click Refresh button, When status of this dataset is in 'READY' state, you can now start chat conversation with this assistant.
8.  If any error occours, move mouse to the status field, the error message will be shown in tooltip.
9.  The Size field will display how much size of this file uploaded, the Data trained field will show how much size(characters) learnd by LLM.


### Why Data trained size is larger than the file size uploaded?

Due the embedding technology, for a new file, we will spilt your documents into text chunks at a fixed size. For better search result, we also add an overlap size to each chunk, the default overlap size is 10 bytes, thus the total data size trained will be the file size + total chunks * 10. The dataset limit in subscription plan is based on this value, total data trained size.


### Why Data trained size is 0 or smaller than file size uploaded?

We also use the cumulative value of all datasets uploaded to this assistant. For example, if you have two pdf files, pdf1 and pdf2, and the content of pdf2 is a clone or subset of pdf1, in this case, when we detected a document chunk has been already learned by this assistant, the data trained size will not include this document chunk, only newly added document will be learned by assistant, so the data trained size only include newly learned document size. 

Note, when you delete a base dataset that referenced by other datasets of this assistant, the memory from this dataset will be erased, even though the other datasets may contains the same memory, so pay attation to the order of datasets of this assistant when removing.


