# BOMHUB API DOCUMENT 


Server: https://bomhub.vercel.app

Product: https://beta-bomhub.web.app


1. GET Banner Items (Dữ liệu dùng cho banner)

- Url : /api/film

- Query Params : Empty

- Body Data : Empty


2. GET Top Trending

- Url: /api/film/trending

- Query Params : Empty

- Body Data : Empty


3. GET TV Show / Movie Detail

- Url : /api/film/detail

- Query Params : { id, type } 

  + id: Mã phim
  
  + type: 0 = Movie (Phim lẻ) | 1 = TV Show (Phim truyền hình) (1*)

- Body Data : Empty


4. GET Stream (Nhận 1 hls media src, trên Client dùng HLS Player để có thể chạy được video)

- Url : /api/film/stream

- Query Params : { type, id, eid, definition }

  + type : Xem chú thích (1*)
  
  + id : Mã phim
  
  + eid : Mã tập phim
  
  + definition : GROOT_HD = 1080p, GROOT_SD = 720p, GROOT_LD = 540p
  
- Body Data : Empty


5. POST 

- Url : api/film/basic-search

- Query Params : Empty

- Body Data: { keyword, size }
