# strings-vs-bytes

Test results on my Apple M1 Pro (10 cores):

```bash
go test -bench=.

BenchmarkBytesToStrings-10              100083099               11.79 ns/op           24 B/op          1 allocs/op
BenchmarkBytesCompareSame-10            547281720                2.204 ns/op           0 B/op          0 allocs/op
BenchmarkBytesCompareDifferent-10       535047963                2.221 ns/op           0 B/op          0 allocs/op
BenchmarkStringsCompareSame-10          396920886                3.017 ns/op           0 B/op          0 allocs/op
BenchmarkStringsCompareDifferent-10     213098088                5.631 ns/op           0 B/op          0 allocs/op
BenchmarkBytesContains-10               142130079                8.442 ns/op           0 B/op          0 allocs/op
BenchmarkStringsContains-10             145400233                8.145 ns/op           0 B/op          0 allocs/op
BenchmarkBytesIndex-10                  359981505                3.335 ns/op           0 B/op          0 allocs/op
BenchmarkStringIndex-10                 366940635                3.265 ns/op           0 B/op          0 allocs/op
BenchmarkBytesReplace-10                28265804                41.64 ns/op           24 B/op          1 allocs/op
BenchmarkStringsReplace-10              25634749                46.49 ns/op           24 B/op          1 allocs/op
BenchmarkBytesConcat2-10                71050237                16.89 ns/op           32 B/op          1 allocs/op
BenchmarkStringsConcat2-10              52257506                22.39 ns/op           32 B/op          1 allocs/op
BenchmarkStringsJoin2-10                45807208                25.60 ns/op           32 B/op          1 allocs/op
BenchmarkMapHints-10                    290136886                4.038 ns/op           0 B/op          0 allocs/op
BenchmarkMapsHints_Dont-10              177106510                6.602 ns/op           0 B/op          0 allocs/op
```

### Link :
https://medium.com/@felipedutratine/in-golang-should-i-work-with-bytes-or-strings-8bd1f5a7fd48#.6m2j7ssec
