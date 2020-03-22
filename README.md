# redis-at-glance
Learn redis express way


###### What is it?


> In memory data storage. 


###### Is it secure?


> Since it is in-memory redis is designed to be used only by trusted clients. Yes it is secure.


###### why use redis?

> For fast store and retrieval of data. Redis supports multiple data structures, string, integer, list and more. Redis store data as key value mapping. 

## Commands for redis
> - GET KEYNAME
> - SET KEYNAME2 SOMEVALUE

Set expiration to existing key
> - SET EXPIRATION KEYNAME SOMEVALUE_INSECONDS
> - SETEX KEYNAME SOMEVALUE_INSECONDS

Initialise and set expiration
> - SETEX KEYNAME SOMEVALUE_INSECONDS SOMEVALUE


> - TTL SOMEKEY_SETTEDWITHEXPIRATION
> - PERSIST SOMEKEY_SETTEDWITHEXPIRATION
> - MSET KEY1 VALUE1 KEY2 VALUE2
> - APPEND KEY1 APPENDVALUE_TO_OLDVALUE
> - RENAME KEY1 NEWKEYNAME

Remove all key value from redis
> FLUSHALL

List structure
> - LPUSH
> - LPUSH LISTNAME "VALUE 1"
> - LPUSH LISTNAME "VALUE 2"
> - LPUSH LISTNAME "VALUE 3"
> - RPUSH LISTNAME "VALUE_PUSHED_AT_LAST_POSITION"

Fetch all elements from list
> - LRANGE LISTNAME 0 -1

Fetch 2nd and 3rd elements
> - LRANGE LISTNAME 1 2

Length of list
> - LLEN LISTNAME

> - LPOP LISTNAME
> - RPOP LISTNAME

Set structure
> - SADD SETNAME "VALUE1"
> - SADD SETNAME "VALUE2"
> - SISMEMBER SETNAME "VALUE TO CHECK IF PRESENT"
> - SMEMBERS SETNAME
> - SCARD SETNAME ( WILL RETURN NO OF ELEMENTS IN SET)
> - SREM SETNAME "VALUE_TO_REMOVE"
