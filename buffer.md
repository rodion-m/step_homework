# Буфер обмена
 ```charp
 List<Span<int>> results = new();
s = s.ToSpan();
for(int a = 0; a < s.Length; a++) {
    var chr = s[a];
    if(dict.Contains(chr)) {
        var remains = s[a..s.Length-1];
        if(dict.All(d => remains.Contains(d))) {
            results.Add(remains);
        }
    }
}

return results.OrderBy(it => it.Length).First();
 ```
