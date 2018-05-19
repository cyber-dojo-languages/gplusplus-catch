FROM  cyberdojofoundation/gplusplus
LABEL maintainer=jon@jaggersoft.com

RUN cd /usr/include/ \
  && curl \
       --remote-header-name  `# -J Use the header-provided filename` \
       --location            `# -L Follow redirects` \
       --remote-name         `# -O Write output to a file named as the remote file` \
         https://raw.githubusercontent.com/catchorg/Catch2/master/single_include/catch.hpp

COPY red_amber_green.rb /usr/local/bin
