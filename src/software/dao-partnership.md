---
layout: page
title: The DAO Partnership
permalink: /software/dao-partnership/
---
While the [Slock.It DAO][1] was [imploding][2], a colleague and I decided we needed our own _Distributed Autonomous Organization_ - a partnership on the [Ethereum blockchain][3]. We took the Slock.It code and modified it to allow a fixed number of partners instead of an arbitrary float of crowd-sourced funds.

It functions the same way, though without the "re-entrancy" issue that affected the Slock.It DAO. One of the pre-defined partners proposes an Ethereum transaction. The remaining partners then have an opportunity to "vote" in support of the transaction. If all partners vote, the transaction can then be executed by the partnership contract.

The fun bit of course is that these transactions can be much more than simple ETH transfers. They can be arbitrary blobs of pre-compiled EVM bytecode, turning an executed transaction into a call into another contract - or back into itself.

The purpose of the partnership at the moment is unclear, but it bridges the gap between my colleague in Spain and I in Canada, and gives us a platform to grow blockchain experiments on the fascinating and world-changing Ethereum network.

You can find the DAO Partnership code on [GitHub][4].

[1]: https://daohub.org/
[2]: http://www.coindesk.com/understanding-dao-hack-journalists/
[3]: https://www.ethereum.org/
[4]: https://github.com/jamiehale/dao_partnership