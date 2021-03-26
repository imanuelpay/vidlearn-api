# VidLearn API
- Base URL = `http://vidlearn.rf.gd/api/v1/`
- Header : 
  - Content-Type: application/json
  - Accept: application/json


## Categories
Request :
- Method : GET
- Endpoint : `/categories`

Response :
```json
{
    "success": true,
    "title": "Categories",
    "data": [
        {
            "#": 1,
            "id": 19,
            "name": "ACCOUNTING",
            "total_playlist": 2,
            "url": "http://vidlearn.rf.gd/api/v1/playlist?category=accounting&id_category=19"
        }
    ],
    "meta": {
        "total": 5,
        "count": 5,
        "per_page": 5,
        "total_pages": 1,
        "links": {
            "base_url": "http://vidlearn.rf.gd/api/v1/categories",
            "previous": false,
            "next": false
        }
    }
}
```


## Tags
Request :
- Method : GET
- Endpoint : `/tags`

Response :
```json
{
    "success": true,
    "title": "Tags",
    "data": [
        {
            "#": 1,
            "id": 71,
            "name": "ACCOUNTING",
            "total_playlist": 1,
            "url": "http://vidlearn.rf.gd/api/v1/playlist?tag=accounting&id_tag=71"
        }
    ],
    "meta": {
        "total": 5,
        "count": 5,
        "per_page": 5,
        "total_pages": 1,
        "links": {
            "base_url": "http://vidlearn.rf.gd/api/v1/tags",
            "previous": false,
            "next": false
        }
    }
}
```


## Playlists
Request :
- Method : GET
- Endpoint : `/playlist`

Response :
```json
{
    "success": true,
    "title": "Playlists",
    "data": [
        {
            "#": 1,
            "id": 36,
            "name": "CCNA - Network Engineer",
            "author": "Imanuel Pay",
            "thumbnail": "http://vidlearn.rf.gd/images/thumbnail/ccna-network-engineer-1614602053.png",
            "description": "Dokumentasi Belajar Cisco CCNA Network Engineer.....",
            "created_at": "2021-03-01 20:08:15",
            "created_at_date_format": "Monday, 01 March 2021 08:08:15 PM",
            "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36"
        }
    ],
    "meta": {
        "total": 5,
        "count": 5,
        "per_page": 5,
        "total_pages": 1,
        "links": {
            "base_url": "http://vidlearn.rf.gd/api/v1/playlist",
            "previous": false,
            "next": false
        }
    }
}
```


## Show Playlist
Request :
- Method : GET
- Endpoint : `/playlist?show={slug}&id={id}`

Response :
```json
{
    "success": true,
    "title": "Show playlist CCNA - Network Engineer",
    "data": {
        "id": 36,
        "name": "CCNA - Network Engineer",
        "thumbnail": "http://vidlearn.rf.gd/images/thumbnail/ccna-network-engineer-1614602053.png",
        "description": "Dokumentasi Belajar Cisco CCNA Network Engineer",
        "created_at": "2021-03-01 20:08:15",
        "created_at_date_format": "Monday, 01 March 2021 08:08:15 PM",
        "videos": [
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #1",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-1&id_video=78"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #2",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-2&id_video=79"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #3",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-3&id_video=80"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #4",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-4&id_video=81"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #5",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-5&id_video=82"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #6",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-6&id_video=83"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #7",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-7&id_video=84"
            },
            {
                "name": "belajar CISCO CCNA Network Engineer bagian #8",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36&video=belajar-cisco-ccna-network-engineer-bagian-8&id_video=85"
            }
        ],
        "category": {
            "name": "IT NETWORK",
            "url": "http://vidlearn.rf.gd/api/v1/playlist?category=it-network&id_category=16"
        },
        "tags": [
            {
                "name": "CISCO",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?tag=cisco&id_tag=66"
            },
            {
                "name": "NETWORK",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?tag=network&id_tag=67"
            },
            {
                "name": "SERVER",
                "url": "http://vidlearn.rf.gd/api/v1/playlist?tag=server&id_tag=64"
            }
        ],
        "author": {
            "name": "Imanuel Pay",
            "profile": "http://vidlearn.rf.gd/images/avatar/imanuel-pay-1614948732.png",
            "description": "Seorang Mahasiswa Ilmu Komputer, Universitas Nusa Cendana. Full Stack Developer & Remote Worker salah satu perusahaan asal Australia. Senang dengan teknologi baru. Laravel addict yang tidak fanatik. Merekam jejak dengan menulis."
        }
    }
}
```


## Wacth Video
Request :
- Method : GET
- Endpoint : `playlist?show={slug_playlist}&id={id_playlist}&video={slug_video}&id_video={id_video}`

Response :
```json
{
    "success": true,
    "title": "CCNA - Network Engineer - belajar CISCO CCNA Network Engineer bagian #1",
    "data": {
        "title": "belajar CISCO CCNA Network Engineer bagian #1",
        "playlist": "CCNA - Network Engineer",
        "link_watch": "https://www.youtube.com/embed/watch?v=0z7LQL2pRe0&list=PLJGji3QDg91Grv-oT6bN51nKdpmvg_v-i&index=1",
        "link_playlist": "http://vidlearn.rf.gd/api/v1/playlist?show=ccna-network-engineer&id=36",
        "description": "Dokumentasi Belajar Cisco CCNA Network Engineer\r\nSupport terus, dengan share video ini, like, dan subscribe,...\r\ndan berikan kritik, masukkan dan sarannya bro..."
    }
}
```
