# tomorrow lab

This GitHub repository is a blog I created using the tool called Quora. The content covered in this blog primarily consists of useful Python and R code in the field of bioinformatics. Since many ideas are borrowed from others, feel free to edit or distribute it, and I thank the original authors whose ideas I've borrowed.

## Preview

It's always a good idea to preview the blog before publish it.

```
quarto preview
```

## Publishing

Once you have configured the source branch and updated your .gitignore, navigate to the directory where your project / git repository is located, make sure you are not on the gh-pages branch, and execute the quarto publish command for GitHub Pages:

```
quarto publish gh-pages
```

The publish command will confirm that you want to publish, render your content, copy the output to a special gh-pages branch, push that branch to GitHub, and then open a browser to view your site once it is deployed.

# 참고 사이트

- https://publickrbook.com/
- https://www.lostineconomics.com/