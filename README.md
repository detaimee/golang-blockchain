# golang-blockchain

<pre>

**>go run main.go createwallet**
New address is: 1KdA3MrFGjXHM5pWueiPQRDaryfUXFQxGx


**> go run main.go createwallet**
New address is: 1McyaF8F7KUGUSagUntQfsTWPvUe1Mqiqg


**> go run main.go createblockchain -address 1McyaF8F7KUGUSagUntQfsTWPvUe1Mqiqg**
badger 2020/06/30 17:24:08 INFO: All 0 tables opened in 0s
Genesis is proved
badger 2020/06/30 17:24:09 DEBUG: Storing value log head: {Fid:0 Len:42 Offset:623}
badger 2020/06/30 17:24:09 INFO: Got compaction priority: {level:0 score:1.73 dropPrefix:[]}
badger 2020/06/30 17:24:09 INFO: Running for level: 0
badger 2020/06/30 17:24:09 DEBUG: LOG Compact. Added 3 keys. Skipped 0 keys. Iteration took: 0s
badger 2020/06/30 17:24:09 DEBUG: Discard stats: map[]
badger 2020/06/30 17:24:09 INFO: LOG Compact 0->1, del 1 tables, add 1 tables, took 2.9864ms
badger 2020/06/30 17:24:09 INFO: Compaction for level: 0 DONE
badger 2020/06/30 17:24:09 INFO: Force compaction on level 0 done
Finished!


**> go run main.go printchain**
badger 2020/06/30 17:26:28 INFO: All 1 tables opened in 1ms
badger 2020/06/30 17:26:28 INFO: Replaying file id: 0 at offset: 665
badger 2020/06/30 17:26:28 INFO: Replay took: 0s
badger 2020/06/30 17:26:28 DEBUG: Value log discard stats empty
Prev. hash: 
Hash: 000bd4f6345df4aaa2d314436ab0ef6808eddf69367aa530425964efc24f5542
PoW: true
--- Transaction 45f1b9407ea562f683fecfe6186681f1e4f506b63900960ba2687b86fa441102:
     Input 0:
       TXID:
       Out:       -1
       Signature:
       PubKey:    4669727374205472616e73616374696f6e2066726f6d2047656e65736973
     Output 0:
       Value:  100
       Script: e2304c9ad500db612635c04b16454b501622969d

badger 2020/06/30 17:26:28 INFO: Got compaction priority: {level:0 score:1.73 dropPrefix:[]}


**> go run main.go send -to 1KdA3MrFGjXHM5pWueiPQRDaryfUXFQxGx 
-from 1McyaF8F7KUGUSagUntQfsTWPvUe1Mqiqg -amount 30**
badger 2020/06/30 17:28:16 INFO: All 1 tables opened in 1ms
badger 2020/06/30 17:28:16 INFO: Replaying file id: 0 at offset: 665
badger 2020/06/30 17:28:16 INFO: Replay took: 0s
badger 2020/06/30 17:28:16 DEBUG: Value log discard stats empty
000aaae257d2a4af140b2b8f72e589dd155e7c158ae2521093988e25728ecfe2
Success!
badger 2020/06/30 17:28:16 DEBUG: Storing value log head: {Fid:0 Len:42 Offset:1480}
badger 2020/06/30 17:28:16 INFO: Got compaction priority: {level:0 score:1.73 dropPrefix:[]}
badger 2020/06/30 17:28:16 INFO: Running for level: 0
badger 2020/06/30 17:28:16 DEBUG: LOG Compact. Added 6 keys. Skipped 0 keys. Iteration took: 0s
badger 2020/06/30 17:28:16 DEBUG: Discard stats: map[]
badger 2020/06/30 17:28:16 INFO: LOG Compact 0->1, del 2 tables, add 1 tables, took 2.9885ms
badger 2020/06/30 17:28:16 INFO: Compaction for level: 0 DONE
badger 2020/06/30 17:28:16 INFO: Force compaction on level 0 done


**> go run main.go printchain**
badger 2020/06/30 17:28:26 INFO: All 1 tables opened in 1ms
badger 2020/06/30 17:28:26 INFO: Replaying file id: 0 at offset: 1522
badger 2020/06/30 17:28:26 INFO: Replay took: 0s
badger 2020/06/30 17:28:26 DEBUG: Value log discard stats empty
Prev. hash: 000bd4f6345df4aaa2d314436ab0ef6808eddf69367aa530425964efc24f5542
Hash: 000aaae257d2a4af140b2b8f72e589dd155e7c158ae2521093988e25728ecfe2
PoW: true
--- Transaction ab47a9716220bcc4acefbd0d5816e8af1a97efae575a3cf31a3d3bccac725057:
     Input 0:
       TXID:     45f1b9407ea562f683fecfe6186681f1e4f506b63900960ba2687b86fa441102
       Out:       0
       Signature: f29f761a17b592425228a51c063093f106cfd1325391845eb6379f0df50b090dbb756d41670ad2e62c982927aec90da78ed578fc6596e6478a6db009b866cee6
       PubKey:    e1ea499b1a8ad42d367c8eb91e34013ce840c1a18955649635d074a577c47cb834349d842cf175727bdeece158ac38732458672d2706e84003ee1b8512bd0e1d
     Output 0:
       Value:  30
       Script: cc48c917574f9c28b817b5b6be75d4b1e9909299
     Output 1:
       Value:  70
       Script: e2304c9ad500db612635c04b16454b501622969d

Prev. hash:
Hash: 000bd4f6345df4aaa2d314436ab0ef6808eddf69367aa530425964efc24f5542
PoW: true
--- Transaction 45f1b9407ea562f683fecfe6186681f1e4f506b63900960ba2687b86fa441102:
     Input 0:
       TXID:
       Out:       -1
       Signature:
       PubKey:    4669727374205472616e73616374696f6e2066726f6d2047656e65736973
     Output 0:
       Value:  100
       Script: e2304c9ad500db612635c04b16454b501622969d

badger 2020/06/30 17:28:26 INFO: Got compaction priority: {level:0 score:1.73 dropPrefix:[]}

</pre>
