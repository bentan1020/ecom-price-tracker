## Pricewise

### Features
- [x] Track amazon product prices
- [x] Notify users whenever an amazon item's price drops
- [x] Enter an amazon product link and you'll see all of it's history

![Screenshot 2023-11-05 at 6 04 04 PM](https://github.com/bentan1020/priceWise/assets/73725152/49b9db74-5d55-4d56-a7fc-39215aa77d2f)

### Tech Stack
- MongoDB
- NextJS (Typescript)
- Tailwind
- HeadlessUI
- Cheerio

### To start this project
1. Go to `.env.sample`
2. Enter all of your credentials and the appropriate API keys
3. Go to terminal, run `npm install`
4. `npm run dev`

### Notes/Challenges:
- Differences between server and client components
    - https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns
- Responsive carousel library package
    - https://www.npmjs.com/package/react-responsive-carousel
- Cheerio - a tool to parse HTML and XML pages
    - to get the ID of something, let's say the title
        - Inspect element
        - Usually it's span#productTitle on Amazon
        - productTitle is the id of that span
        - scrape it like this: const title = $('#productTitle').text().trim();
