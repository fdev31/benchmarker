###########################
Compression tools benchmark
###########################

Personal interpretation
#######################

xz
    For highest compression ratio at cost of speed
lz4
    For the fastest, but moderate results
(p)zstd
    For everything in the middle


Files
#####

13MB -- mix_pdf_jpg.tar
    A mix of pdf & jpg documents (hard to compress)
41MB -- etc_files.tar
    All files on my /etc filesystem
46MB -- journal.log
    systemctl's journalct output
94MB -- robot.blend
    Some uncompressed .blend file
80MB -- usr_bin_xstar.tar
    Tarball of /usr/bin/x* filesystem

Results
#######

.. note::

    - Each point is a compressed file
    - Same input file = same color
    - Same shape = same compressor (each point are linked with a line)
    - **click on pictures for bigger & interactive version**

.. image:: default_compression.png
    :target: https://cdn.rawgit.com/fdev31/benchmarker/9303e70f/default_compression.html

.. image:: max_compression.png
    :target: https://cdn.rawgit.com/fdev31/benchmarker/9303e70f/max_compression.html

.. image:: decompression.png
    :target: https://cdn.rawgit.com/fdev31/benchmarker/9303e70f/decompression.html

Do it yourself
##############

- Install plotly for Python
- Copy your archives or files to ``files``
- run ``./run``
