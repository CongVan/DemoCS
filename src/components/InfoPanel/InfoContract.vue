<template>
<v-container fluid="" pa-0>
    <v-card>
        <v-layout row="" wrap="" pl-2>
            <v-flex lg3 px-3>
                <v-layout row>
                    <!-- <v-flex lg5 >
                    <v-subheader px-0>Vùng miền/ chi nhánh</v-subheader>
                </v-flex> -->
                    <v-flex lg6 pr-2>
                        <v-text-field label="Vùng miền" placeholder="Vùng 5" mb-0>
                        </v-text-field>
                    </v-flex>
                    <v-flex lg6>
                        <v-text-field label="Chi nhánh" placeholder="HCM" mb-0>
                        </v-text-field>
                    </v-flex>
                </v-layout>
                <v-layout row>
                    <v-flex lg6 pr-2>
                        <v-text-field label="Gói dịch vụ" placeholder="FTTH-F2">
                        </v-text-field>
                    </v-flex>
                    <v-flex lg6>
                        <v-text-field label="Gói tính cước" placeholder="FTTH-F3">
                        </v-text-field>
                    </v-flex>
                </v-layout>
                <v-layout row>
                    <v-flex lg6 pr-2>
                        <v-text-field label="Số hợp đồng" placeholder="SGD0000001">
                        </v-text-field>
                    </v-flex>
                    <v-flex lg6>
                        <v-text-field label="Ngày hợp đồng" placeholder="01-01-2019">
                        </v-text-field>
                    </v-flex>
                </v-layout>
                <v-layout row>
                    <v-flex lg12>
                        <v-text-field label="Tên khách hàng" placeholder="Nguyễn Văn A">
                        </v-text-field>
                    </v-flex>
                </v-layout>
                <v-layout row>
                    <v-flex lg6 pr-2>
                        <v-text-field label="Đối tượng KH" placeholder="VIP1">
                        </v-text-field>
                    </v-flex>
                    <v-flex lg6>
                        <v-text-field label="Độ tuổi SD" placeholder="12 tháng">
                        </v-text-field>
                    </v-flex>
                </v-layout>
                <v-layout row>
                    <v-flex lg12>
                        <v-text-field label="Chi tiết đối tượng KH" placeholder="Nhà báo">
                        </v-text-field>
                    </v-flex>
                </v-layout>
            </v-flex>
            <v-flex lg9>
                <v-layout>
                    <v-flex lg4 px-3>
                        <v-layout row>
                            <v-flex lg6 pr-2>
                                <v-text-field label="Tình trạng Internet" placeholder="Bình thường">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg6>
                                <v-text-field label="Ngày cập nhật" placeholder="01-01-2019">
                                </v-text-field>
                            </v-flex>
                        </v-layout>
                        <v-layout row>
                            <v-flex lg6 pr-2>
                                <v-text-field label="Tình trạng truyền hình" placeholder="Bình thường">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg6>
                                <v-text-field label="Ngày cập nhật" placeholder="01-01-2019">
                                </v-text-field>
                            </v-flex>
                        </v-layout>
                        <v-layout row>
                            <v-flex lg12>
                                <v-text-field label="Địa chỉ lắp đặt" placeholder="HCM">
                                </v-text-field>
                            </v-flex>
                        </v-layout>
                        <v-layout row>
                            <v-flex lg12>
                                <v-text-field label="Địa chỉ thanh toán" placeholder="HCM">
                                </v-text-field>
                            </v-flex>
                        </v-layout>
                    </v-flex>
                    <v-flex lg8>
                        <v-layout>
                            <v-flex lg2 justify-center>
                                <v-icon x-large color="red"> warning</v-icon>
                            </v-flex>
                            <v-flex lg8>
                                <v-btn color="primary" ma-0 dark v-for="i in 6" :key="i">Accept
                                    <v-icon dark right>check_circle</v-icon>
                                </v-btn>
                            </v-flex>
                        </v-layout>
                        <v-layout row>
                            <v-flex lg12>
                                <v-textarea label="Lưu ý CSKH" rows="2" color="red" value="The Woodman set to work at once, and so sharp was his axe that the tree was soon chopped nearly through."></v-textarea>
                            </v-flex>
                        </v-layout>
                        <v-layout row>
                            <v-flex lg6 pr-2>
                                <v-text-field label="Bộ phận ghi nhận" placeholder="CUS">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg6>
                                <v-text-field label="Thời gian ghi nhận" placeholder="01-01-2019">
                                </v-text-field>
                            </v-flex>
                        </v-layout>
                    </v-flex>
                </v-layout>
                <v-layout column >
                    <v-card class="pa-2" color="grey lighten-4">
                        <v-layout row="" color="red">
                            <v-flex lg3 pr-2 class="error--text">
                                <v-text-field color="red" class="error--text"  label="Thiết bị lỗi" placeholder="HCM_123123-12CCN">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="Mã lỗi" placeholder="SC1231231231">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="TG sự cố" placeholder="01-01-2019">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="TG DK kết thúc" placeholder="01-01-2019">
                                </v-text-field>
                            </v-flex>

                        </v-layout>
                        <v-layout row="">
                            <v-flex lg3 pr-2>
                                <v-text-field label="Nguyên nhân" placeholder="Chưa xác định">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="Kết quả" placeholder="KH bị ảnh hưởng">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="Tình trạng" placeholder="Tiếp nhận">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-text-field label="Queue" placeholder="INF">
                                </v-text-field>
                            </v-flex>
                            <v-flex lg3 pr-2>
                                <v-switch input-value="true" label="SMS" color="success" value="true" hide-details></v-switch>
                            </v-flex>
                        </v-layout>
                    </v-card>

                </v-layout>
            </v-flex>

        </v-layout>
    </v-card>
</v-container>
</template>

<script>
export default {
    props: ['Contract'],
    name: 'InfoContract'
}
</script>

<style>

</style>
