#include <bits/stdc++.h>
using namespace std;

int main() {

    int N;
    long long K;
    if (!(cin >> N >> K)) return 0;

    vector<long long> a(N);
    for (int i = 0; i < N; ++i) cin >> a[i];

    unordered_map<long long, long long> count;
    long long pref = 0;
    long long ans = 0;

    count[0] = 1;

    for (int i = 0; i < N; ++i) {
        pref += a[i];
    
        if (count.find(pref - K) != count.end()) ans += count[pref - K];
        ++count[pref];
    }

    cout << ans << '\n';
    return 0;
}
