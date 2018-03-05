BioVM - A virtual machine for Bioinformatics
============================================
BioVM_ is a virtual machine based on
Ubuntu MATE Linux 16.04 with pre-installed and
pre-configured software for Bioinformatics. It is the successor
to the VLinux_ live CD originally released in 2004.

.. figure:: https://vimal.io/2018/images/biovm-menu.png
   :alt: The menu contains a Bioinformatics category


Get BioVM
---------

.. raw:: html	 	 

	 <a class="gumroad-button" href="https://gum.co/JXPmw" target="_blank">Get BioVM Free</a> |

	 <a class="gumroad-button" href="https://gum.co/htNi" target="_blank">Get BioVM Personal</a> |

	 <a class="gumroad-button" href="https://gum.co/wWqE" target="_blank">Get BioVM Business</a>
	 
Features
--------

* A minimal installation of Ubuntu Linux
* Pre-installed Bioinformatics software - Bedtools_, `Bowtie 2`_,
  BWA_, ClustalO_, Cutadapt_, EMBOSS_ (with the Jemboss and
  Emboss Explorer graphical user interfaces and the EMBASSY
  packages), FastQC_, FASTX-Toolkit_, Mummer_, Muscle_,
  `NCBI BLAST+`_, `Primer 3`_, Samtools_, Tophat_, TreeviewX_,
  Trimmomatic_, UGENE_.
* A local instance of Galaxy_
* The Conda_ package manager with a base environment setup.
* Use Bioinformatics software distributed as Docker_ images.
* General programming and System tools - gcc, make, git etc., 
* Python, PERL and R language support.

Development notes
-----------------
This virtual machine is built using the :literal:`ubuntu/xenial64`
base image. To build this virtual machine, ensure VirtualBox_,
Vagrant_ and Ansible_ is installed on the host. Then use
the :literal:`vagrant up` command::

  git clone https://github.com/vimalkvn/biovm
  cd biovm
  vagrant up

Tasks are defined as ansible roles. For example, the **biovm-core**
role installs the core Bioinformatics software included in BioVM.
Additional roles can be defined and then included in **setup.yml**.

The Virtual machine is exported manually from VirtualBox (ova).



.. links
   
.. _Ansible: https://www.ansible.com/
.. _BioVM: https://vimal.io/biovm
.. _BioPython: http://biopython.org/
.. _Bedtools: https://bedtools.readthedocs.io
.. _BWA: http://bio-bwa.sourceforge.net/
.. _Bowtie 2: http://bowtie-bio.sourceforge.net/bowtie2/
.. _ClustalO: http://www.clustal.org/omega/
.. _Cutadapt: https://github.com/marcelm/cutadapt
.. _Conda: https://conda.io
.. _Docker: https://www.docker.com/
.. _EMBOSS: http://emboss.sourceforge.net/
.. _FastQC: http://www.bioinformatics.babraham.ac.uk/projects/fastqc/
.. _FASTX-Toolkit: http://hannonlab.cshl.edu/fastx_toolkit/
.. _Galaxy: https://galaxyproject.org
.. _GPLv3: https://www.gnu.org/licenses/gpl-3.0.en.html
.. _Mummer: http://mummer.sourceforge.net/
.. _Muscle: http://www.drive5.com/muscle/
.. _NCBI BLAST+: https://blast.ncbi.nlm.nih.gov/Blast.cgi
.. _Primer 3: http://primer3.sourceforge.net
.. _Samtools: http://samtools.sourceforge.net
.. _Support forums: https://forums.vimal.io/c/biovm
.. _Tophat: http://ccb.jhu.edu/software/tophat
.. _TreeviewX: http://code.google.com/p/treeviewx/
.. _Trimmomatic: http://www.usadellab.org/cms/index.php?page=trimmomatic
.. _UGENE: http://ugene.unipro.ru
.. _Ubuntu MATE: https://ubuntu-mate.org
.. _Vagrant: https://www.vagrantup.com/
.. _VLinux: https://bioinformatics.org/vlinux
.. _VirtualBox: https://www.virtualbox.org/wiki/Downloads


.. PayPal
.. _paypal-custom-donation: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=WSJTBPHTE42DJ
