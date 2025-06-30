wget https://github.com/jgm/pandoc/releases/download/3.7.0.2/pandoc-3.7.0.2-linux-amd64.tar.gz
tar -xf pandoc-3.7.0.2-linux-amd64.tar.gz

sudo apt install texlive soul adjustbox babel-german background bidi collectbox csquotes everypage filehook footmisc footnotebackref framed fvextra letltxmacro ly1 mdframed mweights needspace pagecolor sourcecodepro sourcesanspro titling ucharcat unicode-math upquote xecjk xurl zref draftwatermark

TEXLIVE:
wget https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
tar -xf install-tl-unx.tar.gz
perl /home/ja-latex-test/install-tl-20250630/install-tl -texdir /home/ja-latex-test/texlive/ --scheme=medium --no-interaction
cd 
/home/ja-latex-test/texlive/bin/x86_64-linux/tlmgr install soul adjustbox babel-german background bidi collectbox csquotes everypage filehook footmisc footnotebackref framed fvextra letltxmacro ly1 mdframed mweights needspace pagecolor sourcecodepro sourcesanspro titling ucharcat unicode-math upquote xecjk xurl zref draftwatermark

./pandoc /home/ja-latex-test/OSIR-exam-report-template_OS_v1.md -o /home/ja-latex-test/OSCP-OS-XXXXX-Exam-Report.pdf --from markdown+yaml_metadata_block+raw_html --template /home/ja-latex-test/eisvogel.latex --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src --pdf-engine /home/ja-latex-test/texlive/bin/x86_64-linux/pdflatex

TINYTEX:
wget https://yihui.org/tinytex/TinyTeX.tar.gz
tar -xf TinyTeX.tar.gz
/home/ja-latex-test/.TinyTeX/bin/x86_64-linux/tlmgr install soul adjustbox babel-german background bidi collectbox csquotes everypage filehook footmisc footnotebackref framed fvextra letltxmacro ly1 mdframed mweights needspace pagecolor sourcecodepro sourcesanspro titling ucharcat unicode-math upquote xecjk xurl zref draftwatermark

./pandoc /home/ja-latex-test/OSIR-exam-report-template_OS_v1.md -o /home/ja-latex-test/OSCP-OS-XXXXX-Exam-Report.pdf --from markdown+yaml_metadata_block+raw_html --template /home/ja-latex-test/eisvogel.latex --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src --pdf-engine=/home/ja-latex-test/.TinyTeX/bin/x86_64-linux/pdflatex

wget /home/ja-latex-test/eisvogel_test.latex https://raw.githubusercontent.com/atherton-git/latex-test/refs/heads/main/eisvogel_test.latex
./pandoc /home/ja-latex-test/OSIR-exam-report-template_OS_v1.md -o /home/ja-latex-test/OSCP-OS-XXXXX-Exam-Report.pdf --from markdown+yaml_metadata_block+raw_html --template /home/ja-latex-test/eisvogel_test.latex --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src --pdf-engine=/home/ja-latex-test/.TinyTeX/bin/x86_64-linux/pdflatex

wget /home/ja-latex-test/eisvogel_test.latex https://raw.githubusercontent.com/atherton-git/latex-test/refs/heads/main/eisvogel_test.latex
./pandoc /home/jack/OSIR-exam-report-template_OS_v1.md -o /home/jack/clouddrive/OSCP-Output.pdf --from markdown+yaml_metadata_block+raw_html --template /home/jack/eisvogel_test.latex --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src --pdf-engine=/home/jack/TinyTex/bin/x86_64-linux/pdflatex


INSTALL TEMPLATES:
wget https://raw.githubusercontent.com/atherton-git/latex-test/refs/heads/main/eisvogel.latex
wget https://raw.githubusercontent.com/atherton-git/latex-test/refs/heads/main/eisvogel_test.latex
wget https://raw.githubusercontent.com/noraj/OSCP-Exam-Report-Template-Markdown/refs/heads/master/src/OSIR-exam-report-template_OS_v1.md



./pandoc /home/ja-latex-test/OSIR-exam-report-template_OS_v1.md -o /home/ja-latex-test/intermediary.tex --from markdown+yaml_metadata_block+raw_html --template /home/ja-latex-test/eisvogel.latex --table-of-contents --toc-depth 6 --number-sections --top-level-division=chapter --highlight-style breezedark --resource-path=.:src
