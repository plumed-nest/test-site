**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
Stderr for source:  na/plumed.inp   
(download [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
PairEntropy.cpp: In constructor ‘PLMD::NeighborListParallel::NeighborListParallel(const std::vector<PLMD::AtomNumber>&, const std::vector<PLMD::AtomNumber>&, const bool&, const bool&, const PLMD::Pbc&, PLMD::Communicator&, PLMD::Log&, const double&, const bool&, const int&, const double&)’:
PairEntropy.cpp:65:8: warning: ‘PLMD::NeighborListParallel::mylog’ will be initialized after [-Wreorder]
   65 |   Log& mylog;
      |        ^~~~~
PairEntropy.cpp:54:21: warning:   ‘double PLMD::NeighborListParallel::skin_’ [-Wreorder]
   54 |   double distance_, skin_;
      |                     ^~~~~
PairEntropy.cpp:180:1: warning:   when initialized here [-Wreorder]
  180 | NeighborListParallel::NeighborListParallel(const vector<AtomNumber>& list0, const vector<AtomNumber>& list1,
      | ^~~~~~~~~~~~~~~~~~~~
PairEntropy.cpp:54:21: warning: ‘PLMD::NeighborListParallel::skin_’ will be initialized after [-Wreorder]
   54 |   double distance_, skin_;
      |                     ^~~~~
PairEntropy.cpp:42:8: warning:   ‘bool PLMD::NeighborListParallel::do_full_list_’ [-Wreorder]
   42 |   bool do_full_list_;
      |        ^~~~~~~~~~~~~
PairEntropy.cpp:180:1: warning:   when initialized here [-Wreorder]
  180 | NeighborListParallel::NeighborListParallel(const vector<AtomNumber>& list0, const vector<AtomNumber>& list1,
      | ^~~~~~~~~~~~~~~~~~~~
PairEntropy.cpp: In constructor ‘PLMD::NeighborListParallel::NeighborListParallel(const std::vector<PLMD::AtomNumber>&, const bool&, const PLMD::Pbc&, PLMD::Communicator&, PLMD::Log&, const double&, const bool&, const int&, const double&)’:
PairEntropy.cpp:65:8: warning: ‘PLMD::NeighborListParallel::mylog’ will be initialized after [-Wreorder]
   65 |   Log& mylog;
      |        ^~~~~
PairEntropy.cpp:54:21: warning:   ‘double PLMD::NeighborListParallel::skin_’ [-Wreorder]
   54 |   double distance_, skin_;
      |                     ^~~~~
PairEntropy.cpp:212:1: warning:   when initialized here [-Wreorder]
  212 | NeighborListParallel::NeighborListParallel(const vector<AtomNumber>& list0, const bool& do_pbc,
      | ^~~~~~~~~~~~~~~~~~~~
PairEntropy.cpp:54:21: warning: ‘PLMD::NeighborListParallel::skin_’ will be initialized after [-Wreorder]
   54 |   double distance_, skin_;
      |                     ^~~~~
PairEntropy.cpp:42:8: warning:   ‘bool PLMD::NeighborListParallel::do_full_list_’ [-Wreorder]
   42 |   bool do_full_list_;
      |        ^~~~~~~~~~~~~
PairEntropy.cpp:212:1: warning:   when initialized here [-Wreorder]
  212 | NeighborListParallel::NeighborListParallel(const vector<AtomNumber>& list0, const bool& do_pbc,
      | ^~~~~~~~~~~~~~~~~~~~
PairEntropy.cpp: In member function ‘void PLMD::NeighborListParallel::updateFullListWithLinkedList(const std::vector<PLMD::VectorGeneric<3> >&)’:
PairEntropy.cpp:313:47: warning: variable ‘atombin’ set but not used [-Wunused-but-set-variable]
  313 |        unsigned atombinx, atombiny, atombinz, atombin;
      |                                               ^~~~~~~
PairEntropy.cpp:337:47: warning: variable ‘atombin’ set but not used [-Wunused-but-set-variable]
  337 |        unsigned atombinx, atombiny, atombinz, atombin;
      |                                               ^~~~~~~
PairEntropy.cpp: In member function ‘void PLMD::NeighborListParallel::updateHalfListWithLinkedList(const std::vector<PLMD::VectorGeneric<3> >&)’:
PairEntropy.cpp:377:19: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  377 |              if (j>=i) continue;
      |                  ~^~~
PairEntropy.cpp:371:47: warning: variable ‘atombin’ set but not used [-Wunused-but-set-variable]
  371 |        unsigned atombinx, atombiny, atombinz, atombin;
      |                                               ^~~~~~~
PairEntropy.cpp:395:47: warning: variable ‘atombin’ set but not used [-Wunused-but-set-variable]
  395 |        unsigned atombinx, atombiny, atombinz, atombin;
      |                                               ^~~~~~~
PairEntropy.cpp: In member function ‘void PLMD::NeighborListParallel::gatherStats(const std::vector<PLMD::VectorGeneric<3> >&)’:
PairEntropy.cpp:496:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  496 |   for(unsigned int i=0;i<mycomm.Get_size();i+=1) allNeighNum+=neighbors_ranks_[i];
      |                        ~^~~~~~~~~~~~~~~~~~
PairEntropy.cpp: In member function ‘virtual void PLMD::colvar::PairEntropy::calculate()’:
PairEntropy.cpp:990:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  990 |            if (minBin > (nhist-1)) minBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
PairEntropy.cpp:992:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  992 |            if (maxBin > (nhist-1)) maxBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
PairEntropy.cpp:1032:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
 1032 |            if (minBin > (nhist-1)) minBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
PairEntropy.cpp:1034:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
 1034 |            if (maxBin > (nhist-1)) maxBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
PairEntropy.cpp:1062:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
 1062 |            if (minBin > (nhist-1)) minBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
PairEntropy.cpp:1064:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
 1064 |            if (maxBin > (nhist-1)) maxBin=nhist-1;
      |                ~~~~~~~^~~~~~~~~~~
</pre>
{% endraw %}
