## v3.3.1 - Complete daily history before upload

- Adds exact training, wage-change, role-change, and hire-history retrieval to Daily sync because each can change during normal daily company activity.
- Collects company news, stale business/employee/stock data, advertisement changes, restocking orders, and staff history before sending anything to the Pythagoras API.
- Uploads one coherent completed daily state so newly discovered restocks and staff-history changes are not left locally until a later sync.
- Keeps manual Business, Employees, Stock, and Staff history sync actions working independently while suppressing nested activity panels and intermediate uploads inside Daily sync.
