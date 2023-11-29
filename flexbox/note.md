+ Các thuộc tính áp dụng cho flex container

- display
- flex-direction
- flex-flow
- flex-wrap

- align-content => Căn chỉnh nội dung theo cross-axis, và chỉ áp dụng nếu có 2 dòng trở lên.
    - stretch: lines stretch to take up all the available space in the container
    - flex-start: lines are placed in the top part of the container
    - flex-end: lines are placed in the bottom part of the container
    - center: lines are centered in the middle of the container
    - space-between: lines are evenly distributed in the container
    - space-around: lines are evenly distributed with equal space around each line

- align-items => Căn chỉnh element theo chiều dọc
    - stretch: items are stretched to fill the container
    - flex-start: items are placed in the top part of the container
    - flex-end: items are placed in the bottom part of the container
    - center: items are centered in the middle of the container
    - baseline: items are aligned such as their baselines align

- justify-content => Căn chỉnh elements theo chiêu ngang
    - flex-start: items are packed toward the container’s left side
    - flex-end: items are packed toward the container’s right side
    - center: items are placed in the center
    - space-between: items are evenly distributed in the line
    - space-around: items are evenly distributed in the line with equal space on both sides of the items
    - space-evenly: items are distributed so that the spacing between any two items is equal

+ Các thuộc tính áp dụng cho flex items

- align-self => Căn chỉnh theo chiều dọc áp dụng cho các item
    - auto: equals to the value specified in the align-items property for the flex container
    - stretch: items are stretched to fill the container, still respecting min-width and max-width properties
    - flex-start: items are placed in the top part of the container
    - flex-end: items are placed in the bottom part of the container
    - center: items are centered in the middle of the container
    - baseline: items are aligned such as their baselines align
- flex
- flex-basis => Xác định kích thước mặc định của mục flex trước khi phân bổ không gian có sẵn.
- flex-grow => Áp dụng khi kích thước item nhỏ hơn kích thước container
    Ví dụ: Container có kích thước 1000
            item_1 có flex-basis = 200px; flex-grow = 3
            item_2 có flex-basis = 400px; flex-grow = 5
            => Total basis: 600px
                Space còn lại container - total basis = 400px
            => item_1 grow 3/8 * 400px = 150px
                item_2 grow 5/8 * 400px = 250px
            =>> Thực tế item_1 có kích thước 350px; item_2 có kích thước 650px.
- flex-shrink => Áp dụng khi tổng kích thước các items lớn hơn container.
    Ví dụ: Container có kích thước 660px
            item_1 có flex-basis: 150px; flex-shrink: 1
            item_2 có flex-basis: 250px; flex-shrink: 2
            item_3 có flex-basis: 350px; flex-shrink: 3
            => Total basis 750px
                Space remaining: -90px
            => ((flex-shrink * flex-basis) / (Total (flex-shrink * flex-basis))) * Space remaining
- order => Sắp xếp thứ tự của các item

11,470588235294118
