# sass-compass-susy

Sass是以程式語言的方式撰寫Css。http://sass-lang.com/ <br>
Compass是強大的Sass編譯工具。http://compass-style.org/ <br>
Susy Power tools for the web。http://susy.oddbird.net/ <br>

# 安裝sass-compass-susy
    1. 打開終端機, 先更新gem
       gem update --system
    2. 安裝sass-compass-susy
       gem install Sass
       gem install compass
       gem install Susy
       (mac要加sudo)
       sudo gem install Sass
       sudo gem install compass
    3. 確認安裝好的版本
       Sass -v
       compass -v
       Susy -v

# 用Compass建立新專案

    ------------------------------------------------------------------------------------
    require 'compass/import-once/activate'
    # Require any additional compass plugins here.
    Encoding.default_external = 'utf-8'
    # Set this to the root of your project when deployed:
    http_path = "/"                   # 你的根目錄位置
    css_dir = "css"                   # 你的CSS資料夾路徑
    sass_dir = "sass"                 # 你的Sass資料夾路徑
    images_dir = "img"                # 你的圖片資料夾路徑
    javascripts_dir = "js"            # 你的js資料夾路徑
    
    # You can select your preferred output style here (can be overridden via the command line):
    # output_style = :expanded or :nested or :compact or :compressed
    # output_style意思則是指你的編譯出來的CSS碼要用哪種方式編譯出來。
    # expanded   = 一般，每行CSS皆會斷行
    # nested     = 有縮進，較好閱讀
    # compact    = 簡潔格式，匯出來的ＣＳＳ檔案大小比上面兩個還小。
    # compressed = 壓縮過的CSS，所有設定都以一行來進行排列。
    
    # To enable relative paths to assets via compass helper functions. Uncomment:
    relative_assets = true
    
    # To disable debugging comments that display the original location of your selectors. Uncomment:
    # 如果你不希望你的CSS碼有註解的話，請將line_comments = false前面的#拿掉，功能便會生效。
    line_comments = false
    
    # If you prefer the indented syntax, you might want to regenerate this
    # project again passing --syntax sass, or you can uncomment this:
    # preferred_syntax = :sass
    # and then run:
    # sass-convert -R --from scss --to sass sass scss && rm -rf sass && mv scss sass
    ------------------------------------------------------------------------------------
