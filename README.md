This is an implementation of MPTFO v15 (MPTP Fast Open Mechanism) in Linux Kernel.
These patches focus on the Initiator and partially on Listener side.

The next options in userspace are available:

a) sendto(..., ..., ..., MSG_FASTOPEN, ..., ...);

b) setsockopt(..., SOL_TCP, TCP_FASTOPEN, ..., ...);

These patches implement Appendix-B of RFC8684 (MPTFO).

We would like to credit Paulo Abeni, Mat Martineau, Matthieu Baerts and
Benjamin Hesmans for advices and ideas that improved these patches.

Signed-off-by: Dmytro Shytyi <dmytro@shytyi.net>

Patch	                                                                                Series	                    A/R/T	Date	        Submitter	        State

[RFC,mptcp-next,v15,5/5] selftests: mptcp: mptfo Initiator/Listener	                    mptcp: Fast Open Mechanism  - - -	13-	2022-11-06	Dmytro Shytyi		New

[RFC,mptcp-next,v15,4/5] mptcp: add TCP_FASTOPEN sock option	                        mptcp: Fast Open Mechanism	- - -	22-	2022-11-06	Dmytro Shytyi		New

[RFC,mptcp-next,v15,3/5] mptcp: add subflow_v(4,6)_send_synack()	                    mptcp: Fast Open Mechanism	- - -	22-	2022-11-06	Dmytro Shytyi		New

[RFC,mptcp-next,v15,2/5] mptcp: implement delayed seq generation for passive fastopen	mptcp: Fast Open Mechanism	- - -	13-	2022-11-06	Dmytro Shytyi		New

[RFC,mptcp-next,v15,1/5] mptcp: introduce MSG_FASTOPEN flag	                            mptcp: Fast Open Mechanism	- - -	13-	2022-11-06	Dmytro Shytyi		New