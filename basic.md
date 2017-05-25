{
    id: autoincrement,
    username: string,
    password: string,
    profile: {
        birthday: date,
        gender: string,
        phone: string,
        city: string,
        state: string,
        country: string,
        about: text,
        bd_vis: boolean,
        gend_vis:boolean,
        phone_vis:boolean,
        city_vis:boolean,
        state_vis:boolean,
        country_vis:boolean
  },
  * username: String
      * Must contain only word characters
  * password: String
      * Must be at least 8 characters
  * state: String
      * Must be 2 characters if country 'US'
}
