---
id: KeyGenHistory
title: KeyGenHistory
---

<div class="contract-doc"><div class="contract"><h2 class="contract-header"><span class="contract-kind">contract</span> KeyGenHistory</h2><p class="base-contracts"><span>is</span> <a href="eternal-storage_OwnedEternalStorage.html">OwnedEternalStorage</a></p><div class="source">Source: <a href="https://github.com/poanetwork/posdao-contracts/blob/v0.1.0/contracts/KeyGenHistory.sol" target="_blank">contracts/KeyGenHistory.sol</a></div></div><div class="index"><h2>Index</h2><ul><li><a href="KeyGenHistory.html#AckWritten">AckWritten</a></li><li><a href="KeyGenHistory.html#PartWritten">PartWritten</a></li><li><a href="KeyGenHistory.html#_setValidatorWrotePart">_setValidatorWrotePart</a></li><li><a href="KeyGenHistory.html#onlyValidator">onlyValidator</a></li><li><a href="KeyGenHistory.html#setValidatorSetContract">setValidatorSetContract</a></li><li><a href="KeyGenHistory.html#validatorSet">validatorSet</a></li><li><a href="KeyGenHistory.html#validatorWrotePart">validatorWrotePart</a></li><li><a href="KeyGenHistory.html#writeAck">writeAck</a></li><li><a href="KeyGenHistory.html#writePart">writePart</a></li></ul></div><div class="reference"><h2>Reference</h2><div class="events"><h3>Events</h3><ul><li><div class="item event"><span id="AckWritten" class="anchor-marker"></span><h4 class="name">AckWritten</h4><div class="body"><code class="signature">event <strong>AckWritten</strong><span>(address validator, bytes ack, uint256 stakingEpoch, uint256 changeRequestCount) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>validator</code> - address</div><div><code>ack</code> - bytes</div><div><code>stakingEpoch</code> - uint256</div><div><code>changeRequestCount</code> - uint256</div></dd></dl></div></div></li><li><div class="item event"><span id="PartWritten" class="anchor-marker"></span><h4 class="name">PartWritten</h4><div class="body"><code class="signature">event <strong>PartWritten</strong><span>(address validator, bytes part, uint256 stakingEpoch, uint256 changeRequestCount) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>validator</code> - address</div><div><code>part</code> - bytes</div><div><code>stakingEpoch</code> - uint256</div><div><code>changeRequestCount</code> - uint256</div></dd></dl></div></div></li></ul></div><div class="modifiers"><h3>Modifiers</h3><ul><li><div class="item modifier"><span id="onlyValidator" class="anchor-marker"></span><h4 class="name">onlyValidator</h4><div class="body"><code class="signature">modifier <strong>onlyValidator</strong><span>() </span></code><hr/></div></div></li></ul></div><div class="functions"><h3>Functions</h3><ul><li><div class="item function"><span id="_setValidatorWrotePart" class="anchor-marker"></span><h4 class="name">_setValidatorWrotePart</h4><div class="body"><code class="signature">function <strong>_setValidatorWrotePart</strong><span>(uint256 _changeRequestCount, address _validator) </span><span>internal </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_changeRequestCount</code> - uint256</div><div><code>_validator</code> - address</div></dd></dl></div></div></li><li><div class="item function"><span id="setValidatorSetContract" class="anchor-marker"></span><h4 class="name">setValidatorSetContract</h4><div class="body"><code class="signature">function <strong>setValidatorSetContract</strong><span>(IValidatorSet _validatorSet) </span><span>public </span></code><hr/><dl><dt><span class="label-modifiers">Modifiers:</span></dt><dd><a href="eternal-storage_OwnedEternalStorage.html#onlyOwner">onlyOwner </a></dd><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_validatorSet</code> - IValidatorSet</div></dd></dl></div></div></li><li><div class="item function"><span id="validatorSet" class="anchor-marker"></span><h4 class="name">validatorSet</h4><div class="body"><code class="signature">function <strong>validatorSet</strong><span>() </span><span>public </span><span>view </span><span>returns  (IValidatorSet) </span></code><hr/><dl><dt><span class="label-return">Returns:</span></dt><dd>IValidatorSet</dd></dl></div></div></li><li><div class="item function"><span id="validatorWrotePart" class="anchor-marker"></span><h4 class="name">validatorWrotePart</h4><div class="body"><code class="signature">function <strong>validatorWrotePart</strong><span>(uint256 _changeRequestCount, address _validator) </span><span>public </span><span>view </span><span>returns  (bool) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_changeRequestCount</code> - uint256</div><div><code>_validator</code> - address</div></dd><dt><span class="label-return">Returns:</span></dt><dd>bool</dd></dl></div></div></li><li><div class="item function"><span id="writeAck" class="anchor-marker"></span><h4 class="name">writeAck</h4><div class="body"><code class="signature">function <strong>writeAck</strong><span>(bytes _ack) </span><span>public </span></code><hr/><dl><dt><span class="label-modifiers">Modifiers:</span></dt><dd><a href="KeyGenHistory.html#onlyValidator">onlyValidator </a></dd><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_ack</code> - bytes</div></dd></dl></div></div></li><li><div class="item function"><span id="writePart" class="anchor-marker"></span><h4 class="name">writePart</h4><div class="body"><code class="signature">function <strong>writePart</strong><span>(bytes _part) </span><span>public </span></code><hr/><dl><dt><span class="label-modifiers">Modifiers:</span></dt><dd><a href="KeyGenHistory.html#onlyValidator">onlyValidator </a></dd><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_part</code> - bytes</div></dd></dl></div></div></li></ul></div></div></div>